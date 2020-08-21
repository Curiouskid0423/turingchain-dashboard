<h1>Turing Chain 網頁軟體設計</h1>
<p>Aug. 20th, 2020</p>
<hr>

## Pages
*   Log-In Page
*   Dashboard
*   404 Page
<hr>

## A.  &nbsp;&nbsp;&nbsp;Functionality 

#### :star: Log-In Page 
- **Description:** 
    - A log-in page for clients. 
    - Upon entering, users would be required to enter a **token** provided by the OPR team to register for an account id (the token would only be used once for registration)
    - The user then create an account (and password, though not required).
    - **Interface component basics**: 
    Log-in window, id column, password (optional), token column 


#### :star: Dashboard
- **Description**: 
This page will contain a collapsable **dashboard** divided into :three: **sections**.
- **Functionalities**: 
    - Instructions upon log-in.
    - Forms and a submit button (or should clients manually inform OPR team when they have completed?)
    - `Section 1 發證資訊`
        - 證書名稱 
        - 證書文案
        - 發證機構全名
        - 發證日期
        - 發證人姓名/職稱
        - 發證機構標誌/發證人簽名檔 (建議png檔/svg檔)
    - `Section 2 證書設計` 
        - 圖形設計範例
        - 使用自有設計 (建議png檔，尺寸大小A3/B3)
        - 備註欄
    - `Section 3 收證人資訊` 
        - 提供樣本表單(內含必須之參數，客戶可另外自行增加參數)
        - 上傳表單（可接受CSV和excel檔，亦可多次上傳，只會儲存最新版本）


- **開發所需之規格** 
Column name / Form type (e.g. text input, png image, excel file...etc) / Size and stringlength limit.


#### :star: 404 Page
- **Description**: Whenever user attempts to access a non-existent page.

<hr>

##### Missing Info
- 填寫時顯示的instructions
- 客戶輸入規格 (檔案大小、種類...etc)



<hr>

## B. &nbsp;&nbsp;&nbsp;Implementation

- **File structures**
    - `public/`
        - `dist/`  
        Contains both output files: **bundle.js** and **styles.css**
        - index.html
    - `src/`
        - `components/` 
        - `reducers/`
        - `actions/`
        - `router/` (only three routes)
        - `selecters/`
        - `styles/`
        - `tests/` (optional)
        - `redux-store/` (optional)
    - package.json
    - webpack and all the other miscell config files
<br>

- React Component Information and Hierarchy
- Data retrieval types from the backend (Harry)
