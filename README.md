# Fake news detecter
## 動機
* 為提供使用者辨別來自海外的資訊真假度，欲設計可透過其提供之圖片、文字訊息偵測資料來源以及真假程度
## 預期結果
* input: 文字、圖片型文字
* model: 
* output: 真假比例、分析原因、用字特性(sentiment易激起閱聽者情緒?)、追溯回新聞最初出處


## 設立新聞媒體的黑白名單(datasets of Real & Fake)
### 白名單: 公視新聞(公廣集團)、報導者(非營利獨立媒體)、台灣事實查核中心(事實查核團隊)、MyGoPen(事實查核團隊)
https://www.storm.mg/
https://global.udn.com/global_vision/index
https://www.thenewslens.com/
### 黑名單: 每日頭條、壹讀、觸擊者、PTT01、
* 是依照什麼來建立名單?
* mygopen: https://www.mygopen.com/p/blog-page_7.html

## 新聞爬蟲

| Title     | Description  |
| ----------|:-------------:|
| Label     | Real = 1, Fake = 0
| Headline  | Headline of News            |
| Link      | url of News |
| Date      | Published Date      |  
| Source    | Source of the news. (One who can verify the claim of the news)| 
| Category  | Category of News            |
| Content   | Article or body of the news |

Category: International, Econamic, Politics, Technology, Finance, Education, Miscellaneous



# Reference
1. https://github.com/tychen5/NLP_FakeNewsDetection/blob/master/src/ProjectManage.md
2. https://docs.google.com/document/d/1I9SWihDkgXx1NCYCsY-0e_XDicAK346PqQu5wMaesd0/edit
3. https://github.com/Rowan1697/FakeNews
   * 主要研究範圍為印度本地
   * 使用共50K筆資料的dataset
   * 模型: CNN, NLP, SVM, 隨機森林
5. https://github.com/cyang03/CHECKED/tree/master/code
  * 研究對象為微博中討論COVID-19相關話題的留言者，其訊息真假判斷
  * 資料集: 344(fake) + 1776(real) = 2120
7. cofact - https://hackmd.io/@mrorz/Hy8T6nreM?type=view
8. cofact - case study: https://beta.hackfoldr.org/cofacts/https%253A%252F%252Fdatastudio.google.com%252Fopen%252F18J8jZYumsoaCPBk9bdRd97GKvi_W5v-r
9. cofact: https://datastudio.google.com/u/0/reporting/18J8jZYumsoaCPBk9bdRd97GKvi_W5v-r/page/mVfZ
10. mygopen - https://www.mygopen.com/p/blog-page_7.html
11. https://paperswithcode.com/paper/user-preference-aware-fake-news-detection
12. https://www.ipshop.xyz/5426.html
13. 報導者:內容農場的流向與生成 https://www.twreporter.org/a/information-warfare-business-content-farm-mission
    * 利用Facebook「CrowdTangle」追蹤內容農場的下游分享平台
    * 利用SEO-鏈輪法騙過google搜尋，使其可保有排序極高的效果，讓使用者更容易點選到內容農場
    * 為了躲過CrowdTangle的查緝，內容農場會透過建立多種網域來逃避
    * 利用創立「自媒體」(e.g. BLUEPOWER, 觸極者, 庶民起義, jonh ce)，與中國媒體一搭一唱--->我認為是最難辨認的
14. 
