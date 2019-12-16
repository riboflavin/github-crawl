## github.com subdomains

[archiveprogram.github.com](https://archiveprogram.github.com)   
[securitylab.github.com](https://securitylab.github.com)  
[github.com](https://github.com)  

## Outside Domains (separate crawls)

[github.community](https://github.community)  
[opensource.guide](https://opensource.guide)  
[github.blog](https://github.blog)  
[atom.io](https://atom.io)  
[try.github.io](http://try.github.io/)  

## Regex config for github.com  

github.com is huge, so to avoid crawling users or repos, we need to manually compile URLs. [Google Analytics reports help](https://analytics.google.com/analytics/web/#/report/content-pages/a3769691w7201642p7475385/explorer-table.advFilter=%5B%5B0,%22analytics.pagePath%22,%22PT%22,%22%3C%22,1%5D%5D&explorer-table.plotKeys=%5B%5D&explorer-table.rowStart=10&explorer-table.rowCount=1000).

```
https:\/\/github.com\/business.*
https:\/\/github.com\/features.*
https:\/\/github.com\/security.*
https:\/\/github.com\/enterprise.*
https:\/\/github.com\/case-studies.*
https:\/\/github.com\/dashboard.*
https:\/\/github.com\/search.*
https:\/\/github.com\/settings.*
https:\/\/github.com\/explore.*
https:\/\/github.com\/trending.*
https:\/\/github.com\/pricing.*
https:\/\/github.com\/enterprise.*
https:\/\/github.com\/join.*
https:\/\/github.com\/login.*
https:\/\/github.com\/about.*
https:\/\/github.com\/mobile.*
https:\/\/github.com\/notifications.*
https:\/\/github.com\/trending.*
https:\/\/github.com\/logos.*
https:\/\/github.com\/notifications.*
https:\/\/github.com\/customer-stories.*
https:\/\/github.com\/suspended.*
https:\/\/github.com\/orgs.*
https:\/\/github.com\/hc.*
https:\/\/github.com\/nonprofit.*
https:\/\/github.com\/pricing.*
https:\/\/github.com\/marketplace
https:\/\/github.com\/apps
https:\/\/github.com\/collections
https:\/\/github.com\/sponsors
https:\/\/github.com\/topics
```

## Regex config for other domains

```
https:\/\/(gist|help|developer|internships|jobs|enterprise).github.com/
https:\/\/(?!gist|help|developer|internships|jobs|enterprise).*.github.com\/.*
https:\/\/github.community/.*
https:\/\/opensource.guide/.*
https:\/\/github.blog/.*
```

### Notes

Make sure to start the crawl at https://github.com/riboflavin/github-crawl, not github.com
