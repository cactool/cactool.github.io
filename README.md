# Cactool
## Introduction
Cactool is a platform for easy human-coding of social media content from Twitter and TikTok for content analysis. It was designed from the bottom up for researchers who want to code social media content, but don’t need the analytical tools of other platforms – with easy import and exporting of data.

The platform easily lets you contextually analyse a list of social media posts in their native form. Simply import a CSV that contains a list of social media posts (such as collected through NodeXL or other scraping services); another to set your questions; and optionally set user logins, and the platform will do the rest – proving you with an easy to use human-coding platform.

Working through a self-hosted web-app, you can easily create logins for your coders

## Why Cactool

CACT was deigned after one of the creators grew frustrated with how content analysis of social media content was being undertaken. Traditionally, content was collected from Twitter or other formats, scraped, then placed into an Excel spreadsheet for manual coding of the tweets texts. This was obviously frustrating for those wishing to collect and analyse visual data. In addition, such an approach decontextualised the content, removing the content from the styling of the platform.

CACT was designed to get around some of these limitations, while offering researchers a free alternative to expensive commercial products.

## Features
### Easy import & export options
With Cactool, you can import your list of social media posts, and export the coded data back as a CSV for use in your own analysis software (such as SPSS/Excel).

### Visualy friendly
Cactool's easy-to-use web-interface for coders makes coding more accessible, easier, and less monotonous.

### Customisable
You can the platform to show questions you want to be coded for each social media post. Includes options for checkboxes, scales, or open-ended comments. 

### Multi-user
Cactool provides easy to implement options for multiple coders. Separate logins and tagging of which of which content was coded by who for later inter-coder reliability tests. 
## Instalation and Usage
### 1. Download the code
```bash
git clone https://github.com/cactool/cactool/ && cd cactool
```
### 2. Install the requirements
```bash
pip install -Ur requirements.txt
```
### 3. Start the website
```bash
./cactool
```
