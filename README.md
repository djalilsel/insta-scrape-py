# instaPy

instaPy is a Python package designed to help you easily scrape and download Instagram Reels from any public Instagram page. With simple and efficient functionality, insta-scrape-py allows you to extract Reels links from a page, Downlaod reels and downlaod full page reels by providing the username only.

## Features

- **Public Instagram Page Scraping**: Scrape and extract Reels links from any public Instagram profile.
- **Reels Downloading**: Download individual Reels directly to local storage.
- **Full Page Download**: Download all Reels from a specified user by providing their username.
- **Simple Interface**: User-friendly functions for easy interaction and use.
- **Efficient Functionality**: Quickly fetch and download Reels with minimal setup.
- **Error Handling**: Handle errors gracefully, such as when a user’s profile is private or does not exist.
- **Metadata Extraction**: Optionally extract and display metadata related to the Reels, such as captions and view counts.
- **Flexible Integration**: Seamlessly integrate with other Python projects or scripts.

## Installation

You can install insta-scrape-py via pip:

```bash
insta-scrape-py
```

## Example

Make sure to replace the placeholders with the correct values:

```python
from instapy import Instapy

COOKIES = { 'should be json' } # Replace with your instagram cookies
USER = 'username_of_the_page_you_want_to_scrape'
COUNT= 100 # Number of videos you want to download from the page ( you can use float('int') to download all the videos )
PATH = 'path/to/save/videos' # Replace with the path where you want the videos to be saved

# Initialize instapy with the account cookies
insta = Instapy(cookies=COOKIES)

# Scrape a page
insta.scrape_page(USER, count=COUNT, path=PATH)

# Download reels using links
# insta.download_reels(reels_links=['https://www.instagram.com/reels/reel_id/'])
```
