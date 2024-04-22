# Request (RFP) webscraper sitemaps

Scrap formulas to gather the content and attached media/files for all current and archived Requests (RFPs)

## Current requests

#### Media/files
```{"_id":"requests__media","startUrl":["https://www.courts.ca.gov/rfps.htm"],"selectors":[{"id":"requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#mainPanel .container-inlinesearch ul li a","multiple":true,"linkType":"linkFromHref"},{"id":"requests__media","parentSelectors":["requests"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"requests","startUrl":["https://www.courts.ca.gov/rfps.htm"],"selectors":[{"id":"requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#mainPanel .container-inlinesearch ul li a","multiple":true,"linkType":"linkFromHref"},{"id":"title","parentSelectors":["requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"field_rfp_number","parentSelectors":["requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"field_rfp_status","parentSelectors":["requests"],"type":"SelectorHTML","selector":".container-inlinesearch","multiple":false,"regex":"(Notice of Cancellation|Notice of Cancelation)"},{"id":"full_body_content","parentSelectors":["requests"],"type":"SelectorHTML","selector":".container-inlinesearch div.col-xs-12","multiple":false,"regex":""}]}```

---

## Archived requests

### 2023
#### Media/files
```{"_id":"2023_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc76365 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2023_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc76365 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2022
#### Media Files
```{"_id":"2022_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc76364 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2022_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc76364 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2021
#### Media Files
```{"_id":"2021_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc76274 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2021_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc76274 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2020
#### Media Files
```{"_id":"2020_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc76276 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2020_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc76276 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2019
#### Media Files
```{"_id":"2019_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc76275 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2019_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc76275 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2018
#### Media Files
```{"_id":"2018_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc76273 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2018_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc76273 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2017
#### Media Files
```{"_id":"2017_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc76277 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2017_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc76277 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2016
#### Media Files
```{"_id":"2016_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc34449 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2016_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc34449 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2015
#### Media Files
```{"_id":"2015_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc34448 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2015_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc34448 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2014
#### Media Files
```{"_id":"2014_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc26969 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2014_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc26969 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2013
#### Media Files
```{"_id":"2013_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23277 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2013_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23277 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2012
#### Media Files
```{"_id":"2012_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23276 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2012_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23276 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2011
#### Media Files
```{"_id":"2011_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23275 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2011_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23275 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2010
#### Media Files
```{"_id":"2010_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23274 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2010_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23274 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2009
#### Media Files
```{"_id":"2009_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23273 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2009_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23273 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2008
#### Media Files
```{"_id":"2008_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23272 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2008_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23272 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2007
#### Media Files
```{"_id":"2007_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23271 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2007_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23271 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2006
#### Media Files
```{"_id":"2006_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23270 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2006_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23270 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2005
#### Media Files
```{"_id":"2005_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23269 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2005_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23269 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2004
#### Media Files
```{"_id":"2004_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23268 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2004_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23268 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2003
#### Media Files
```{"_id":"2003_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23267 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2003_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23267 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2002
#### Media Files
```{"_id":"2002_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23266 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2002_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23266 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```

---

### 2001
#### Media Files
```{"_id":"2001_archived_requests__media","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests__media","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23265 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests_media__title","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests_media__rfp_id","parentSelectors":["archived_requests__media"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests_media__files","parentSelectors":["archived_requests__media"],"type":"SelectorLink","selector":".container-inlinesearch a[href$=\".pdf\"], .container-inlinesearch a[href$=\".xls\"], .container-inlinesearch a[href$=\".doc\"], .container-inlinesearch a[href$=\".docx\"]","multiple":true,"linkType":"linkFromHref"}]}```

#### Content
```{"_id":"2001_archived_requests","startUrl":["https://www.courts.ca.gov/4834.htm"],"selectors":[{"id":"archived_requests","parentSelectors":["_root"],"type":"SelectorLink","selector":"#acc23265 li a","multiple":true,"linkType":"linkFromHref"},{"id":"archived_requests__title","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"^([^,])+"},{"id":"archived_requests__rfp_id","parentSelectors":["archived_requests"],"type":"SelectorText","selector":"h1","multiple":false,"regex":"(?<=, ).*"},{"id":"archived_requests__body","parentSelectors":["archived_requests"],"type":"SelectorHTML","selector":".container-inlinesearch .col-xs-12","multiple":false,"regex":""}]}```
