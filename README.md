
### API-KEY-REGEX
##### SYSTEM00 SECURITY

#### Artifactory API Token   
```
grep -Po '(?:\s|=|:|"|^)AKC[a-zA-Z0-9]{10,}'
```

#### Artifactory Password 
```
grep -Po '(?:\s|=|:|"|^)AP[\dABCDEF][a-zA-Z0-9]{8,}'
```
#### Authorization Basic   
```
grep -Po 'basic [a-zA-Z0-9_\\-:\\.=]+'
```
####  Authorization Authorization Bearer  
```
grep -Po 'bearer [a-zA-Z0-9_\\-\\.=]+'
```
#### AWS Client ID  
```
grep -Po '(A3T[A-Z0-9]|AKIA|AGPA|AIDA|AROA|AIPA|ANPA|ANVA|ASIA)[A-Z0-9]{16}'
```
#### AWS MWS Key  
```
grep -Po 'amzn\.mws\.[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}'
```
#### AWS Secret Key
```
grep -Po "(?i)aws(.{0,20})?(?-i)['\"][0-9a-zA-Z\/+]{40}['\"]"
```
#### Base32   
```
grep -Po "(?:[A-Z2-7]{8})*(?:[A-Z2-7]{2}={6}|[A-Z2-7]{4}={4}|[A-Z2-7]{5}={3}|[A-Z2-7]{7}=)?"
```
#### Base64  
```
grep -Po "(eyJ|YTo|Tzo|PD[89]|aHR0cHM6L|aHR0cDo|rO0)[a-zA-Z0-9+/]+={0,2}"
```
#### Basic Auth Credentials 
```
grep -Po "(?<=:\/\/)[a-zA-Z0-9]+:[a-zA-Z0-9]+@[a-zA-Z0-9]+\.[a-zA-Z]+"
```
#### Cloudinary Basic Auth 
```
grep -Po "cloudinary:\/\/[0-9]{15}:[0-9A-Za-z]+@[a-z]+"
```
#### Facebook Access Token  
```
grep -Po "EAACEdEose0cBA[0-9A-Za-z]+"
```
#### Facebook Client ID  
```
grep -Po "(?i)(facebook|fb)(.{0,20})?['\"][0-9]{13,17}"
```
#### Facebook Oauth  
```
grep -Po "[f|F][a|A][c|C][e|E][b|B][o|O][o|O][k|K].*['|\"][0-9a-f]{32}['|\"]"
```
#### Facebook Secret Key  
```
grep -Po "(?i)(facebook|fb)(.{0,20})?(?-i)['\"][0-9a-f]{32}"
```
#### Github  
```
grep -Po "(?i)github(.{0,20})?(?-i)['\"][0-9a-zA-Z]{35,40}"
```
#### Google API Key 
```
grep -Po "AIza[0-9A-Za-z\\-_]{35}"
```
#### Google Cloud Platform API Key  
```
grep -Po "(?i)(google|gcp|youtube|drive|yt)(.{0,20})?['\"][AIza[0-9a-z\\-_]{35}]['\"]"
```
#### Google Oauth   
```
grep -Po "[0-9]+-[0-9A-Za-z_]{32}\.apps\.googleusercontent\.com"
```
#### Heroku API Key  
```
grep -Po "[h|H][e|E][r|R][o|O][k|K][u|U].{0,30}[0-9A-F]{8}-[0-9A-F]{4}-[0-9A-F]{4}-[0-9A-F]{4}-[0-9A-F]{12}"
```
#### LinkedIn Secret Key
```
grep -Po "(?i)linkedin(.{0,20})?['\"][0-9a-z]{16}['\"]"
```
#### Mailchamp API Key
```
grep -Po "[0-9a-f]{32}-us[0-9]{1,2}"
```
#### Mailgun API Key 
```
grep -Po "key-[0-9a-zA-Z]{32}"
```
#### Picatic API Key   
```
grep -Po "sk_live_[0-9a-z]{32}"
```
#### Slack Token  
```
grep -Po "xox[baprs]-([0-9a-zA-Z]{10,48})?"
```
#### Slack Webhook 
```
grep -Po "https://hooks.slack.com/services/T[a-zA-Z0-9_]{8}/B[a-zA-Z0-9_]{8}/[a-zA-Z0-9_]{24}"
```
#### Stripe API Key 
```
grep -Po "(?:r|s)k_live_[0-9a-zA-Z]{24}"
```
#### Square Access Token
```
grep -Po "sqOatp-[0-9A-Za-z\\-_]{22}"
```
#### Square Oauth Secret  
```
grep -Po "sq0csp-[ 0-9A-Za-z\\-_]{43}"
```
#### Twilio API Key 
```
grep -Po "SK[0-9a-fA-F]{32}"
```
#### Twitter Oauth  
```
grep -Po "[t|T][w|W][i|I][t|T][t|T][e|E][r|R].{0,30}['\"\\s][0-9a-zA-Z]{35,44}['\"\\s]"
```
#### Twitter Secret Key   
```
grep -Po "(?i)twitter(.{0,20})?['\"][0-9a-z]{35,44}"
```
