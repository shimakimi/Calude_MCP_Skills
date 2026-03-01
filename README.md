# Claude Codeの開発

1. MCPサーバー検証
2. Skillsの動作確認

## 知見を得たものを記載していく

書籍やClaudeとの対話をしたものを参考にコードを書いています。


## Claudeのバージョン

- 2.1.62(Claude Code)


## Claude Skillsの実行

今回はnoteで5080問題をDX化するSkillsを作成した

- skillsディレクトリに移動

```
cd skills
```


- outputフォルダを作成

```
mkdir output
```

- claude codeを起動

```
claude
```

- 記事作成を実行

```
YAMLファイルを読み込んで、MDテンプレートの変数を展開し、                                                                                          
  完成した記事をoutputフォルダに保存してください。   


claude_skills_5080_datascience.yaml を読み込んで、                                                                                                
  note_5080_datascience_dx.md のテンプレートを完成させてください。                                                                                  
                                                                                                                                                    
  条件：                                                                                                                                            
  - {{ }} の変数はYAMLの値で置換                                                                                                                    
  - {% for %} ループはデータで展開                                                                                                                  
  - 文字数は4000字前後                                                                                                                              
  - です・ます調に統一                                                                                                                              
  - output/article_20260228.md として保存      


```