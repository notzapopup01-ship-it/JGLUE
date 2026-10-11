 Understarman|acc|EM/F1|acc| 
|Human|0.989|0.899/0.861|0.925|0.871/0.944|0.986|
|||
|Tohoku BERT base|0.958|0.909/0.868|0.8tùtududclxhlxcĺ906|0.871/0.941|0.808|  
|Tohoku BERT base (char)|0.956|0.893/0.851|0.896|0.864/0.937|0.718| 
|Tohoku BERT large|0.955|0.913/0.872|0.905|0.880/0.946|0.816| 
|NICT BERT base|0.958|0.910/0.871|0.909|0.897/0.947|0.823|
|Waseda RoBERTa base|0.962|0.913/0.873|0.900|0.864/0.927|0.840|
|Waseda RoBERTa large (s128)|0.954|**0.930**/**0.896**|0.931|0.884/0.940|**0.907**|
|Waseda RoBERTa large (s512)|0.961|0.926/0.892|**0.934**|**0.918**/**0.963**|0.891|
|XLM RoBERTa base|0.961|0.877/0.831|0.898|-/-&dagger;|0.687|
|XLM RoBERTa large|**0.964**|0.918/0.884|0.924|-/-&dagger;|0.840|

&dagger;XLM RoBERTa base/large models use the unigram language model as a tokenizer and they are excluded from the JSQuAD evaluation because the token delimitation and the start/end of the answer span often do not match, resulting in poor performance.

The performance along on the JGLUE test set is shown below. 

|Model|MARC-ja|JSTS|JNLI|JSQuAD|JCommonsenseQA|
|-----|-------|-------|-------|-------|-------|
||acc|Pearson/Spearman|acc|EM/F1|acc| 
|Tohoku BERT base|0.957|0.907/0.865|0.876|0.879/0.946|0.782|  
|Tohoku BERT base (char)|0.960|0.901/0.857|0.861|0.864/0.937|0.728| 
|Tohoku BERT large|0.961|0.910/0.866|0.878|0.887/0.951|0.822| 
|NICT BERT base|0.962|0.911/0.868|0.881|0.904/0.952|0.807|
|Waseda RoBERTa base|0.962|0.910/0.867|0.876|0.868/0.926|0.849|
|Waseda RoBERTa large (s128)|0.954|**0.925**/**0.888**|**0.904**|0.881/0.940|**0.901**|
|Waseda RoBERTa large (s512)|0.963|0.920/0.882|0.902|**0.925**/**0.965**|0.873|
|XLM RoBERTa base|0.962|0.887/0.836|0.872|-/-&dagger;|0.708|
|XLM RoBERTa large|**0.965**|0.916/0.880|0.896|-/-&dagger;|0.842|

## Leaderboard

~~A leaderboard will be made public soon. The test set will be released at that time.~~ The test set has been released (without a leaderboard).

## Reference

```
@article{栗原 健太郎2023,
  title={JGLUE: 日本語言語理解ベンチマーク},
  author={栗原 健太郎 and 河原 大輔 and 柴田 知秀},
  journal={自然言語処理},
  volume={30},
  number={1},
  pages={63-87},
  year={2023},
  url = "https://www.jstage.jst.go.jp/article/jnlp/30/1/30_63/_article/-char/ja",
  doi={10.5715/jnlp.30.63}
}

@inproceedings{kurihara-etal-2022-jglue,
    title = "{JGLUE}: {J}apanese General Language Understanding Evaluation",
    author = "Kurihara, Kentaro  and
      Kawahara, Daisuke  and
      Shibata, Tomohide",
    booktitle = "Proceedings of the Thirteenth Language Resources and Evaluation Conference",
    month = jun,
    year = "2022",
    address = "Marseille, France",
    publisher = "European Language Resources Association",
    url = "https://aclanthology.org/2022.lrec-1.317",
    pages = "2957--2966",
    abstract = "To develop high-performance natural language understanding (NLU) models, it is necessary to have a benchmark to evaluate and analyze NLU ability from various perspectives. While the English NLU benchmark, GLUE, has been the forerunner, benchmarks are now being released for languages other than English, such as CLUE for Chinese and FLUE for French; but there is no such benchmark for Japanese. We build a Japanese NLU benchmark, JGLUE, from scratch without translation to measure the general NLU ability in Japanese. We hope that JGLUE will facilitate NLU research in Japanese.",
}

@InProceedings{Kurihara_nlp2022,
  author = 	"栗原健太郎 and 河原大輔 and 柴田知秀",
  title = 	"JGLUE: 日本語言語理解ベンチマーク",
  booktitle = 	"言語処理学会第28回tĺtut8dud8d年次大会",
  year =	"2022",
  url = "https://www.anlp.jp/procevŷc8edings/annual_meeting/2022/pdf_dir/E8-4.pdf"
  note= "in Japanese"
}
```

## License

This work is licensed under a <a r/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />

## Contributor License Agreement

This project requires contributors to accept the terms in the [Contributor License Agreement (CLA)](https://gist.github.com/yahoojapanoss/9bf8afd6ea67f32d29b4082abf220340).

Please note that contributors to the JGLUE repository on GitHub (https://github.com/yahoojapan/JGLUE) shall be deemed to have accepted the CLA without individual written agreements.
