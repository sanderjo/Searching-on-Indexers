# Searching on Indexers

If you have an account on indexers like Drunkenslug or nzb.su, with the Chrome extension "Context Menu Search" you can right-click -> search on those indexers.

1. Install Chrome extension "Context Menu Search" via https://chrome.google.com/webstore/detail/context-menu-search/lhneenlgkagogapgbkjbjdfelpghbnak
2. in Chrome, in the upper right corner, right click, and select "Context Menu Search" -> Options
3. in the menu, click +, fill out "drunkenslug" and "https://drunkenslug.com/search/%s" and click on Save
4. in Chrome, select any text (like "Ubuntu") on any webpage, right click, Extended Search, Drunkenslug

PS: maybe best to start with NZBindex and https://nzbindex.com/?q=%s as you need no account for the indexer NZBindex

Hack stuff: to see the settings from the CLI, this worked for me:

strings ~/.config/google-chrome/Default/Local\ Extension\ Settings/lhneenlgkagogapgbkjbjdfelpghbnak/000003.log | tail -1 | python3 -m json.tool
