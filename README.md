# Rudy Puig

Hi there! Enjoy these goodies...

The following bookmarklet will redirect you to the latest NVIDIA GeForce Game Ready Driver download page. How do you use it? Create a new bookmark in your browser, and use the string below as the URL.

```javascript
javascript:(function(){var url='https://gfwsl.geforce.com/services_toolkit/services/com/nvidia/services/AjaxDriverService.php?func=DriverManualLookup&psid=101&pfid=815&osID=57&languageCode=1033&beta=0&isWHQL=0&dltype=-1&dch=1&upCRD=0&qnf=0&sort1=0&numberOfResults=10';fetch(url).then(res=>res.json()).then(data=>window.location.href=data.IDS[0].downloadInfo.DownloadURL)})()
```