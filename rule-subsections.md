# Rule subsections scrape

This scrape pulls the main content for all the individual rule subsections.

### Content
```{"_id":"rule_subsections","startUrl":["https://www.courts.ca.gov/rules.htm"],"selectors":[{"id":"rule_document_items","parentSelectors":["_root"],"type":"SelectorLink","selector":".container-inlinesearch li > a:nth-of-type(1)","multiple":true,"linkType":"linkFromHref"},{"id":"rule_document_subsections","parentSelectors":["rule_document_items"],"type":"SelectorLink","selector":"li.TOClevel3 a","multiple":true,"linkType":"linkFromHref"},{"id":"rule_subsection_title","parentSelectors":["rule_document_subsections"],"type":"SelectorText","selector":"p.ruleheading","multiple":false,"regex":""},{"id":"rule_subsection_text","parentSelectors":["rule_document_subsections"],"type":"SelectorHTML","selector":"#rulewrapper p[class]:not(.ruleheading)","multiple":false,"regex":""},{"id":"rule_subsection_full_html","parentSelectors":["rule_document_subsections"],"type":"SelectorHTML","selector":"#rulewrapper","multiple":false,"regex":""}]}```
