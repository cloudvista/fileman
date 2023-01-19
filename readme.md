### Fileman documentation

https://www.va.gov/vdl/application.asp?appid=5#top



#### Word to html
```
pandoc -s input/fm22_2um1.docx -t html -c styles.css --extract-media=output/images -o output/fm22_2um1.html 
```


#### Word to markdown
```
pandoc  -s input/fm22_2um1.docx -t markdown --extract-media=output/images -o output/fm22_2um1.md 
```



#### Word to github-friendly markdown
```
pandoc  -s input/fm22_2um1.docx -t gfm --extract-media=output/images -o output/fm22_2um1-gfm.md 
```
