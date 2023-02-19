<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
</head>
<body>
  <h1>badown Documentation</h1>
  <p>badown is a bash script that downloads a random wallpaper from the "top" section of the "wallpapers" subreddit on Reddit. The downloaded wallpaper is saved to a specified directory and set as the desktop wallpaper.</p>

  <h2>Usage</h2>
  <pre><code>badown [-b]</code></pre>
  <p>Use the -b flag to backup the current desktop wallpaper to the specified outpath directory.</p>

  <h2>Dependencies</h2>
  <ul>
    <li>wget</li>
    <li>jq</li>
    <li>feh</li>
  </ul>

  <h2>Installation</h2>
  <p>Make sure the dependencies are installed before running the script. Download the script and make it executable:</p>
  <pre><code>chmod +x badown</code></pre>

  <h2>Options</h2>
  <ul>
    <li><code>-b</code> - backup the current desktop wallpaper</li>
  </ul>

  <h2>Example</h2>
  <p>To download a random wallpaper from the "top" section of the "wallpapers" subreddit, save it to <code>$HOME/img/wallpaper/reddit/</code>,

  <h2>Variables</h2>
  <ul>
    <li><code>JSONCACHE</code> - cache file to save Reddit API response</li>
    <li><code>WPATH</code> - directory where wallpapers are saved</li>
    <li><code>outpath</code> - path to directory where wallpapers are backed up</li>
    <li><code>USERAGENT</code> - user agent to use when getting the JSON from Reddit</li>
    <li><code>APIURL</code> - URL of the API endpoint to get the JSON from Reddit</li>
    <li><code>WJSON</code> - JSON object of the randomly selected wallpaper</li>
    <li><code>CROSSPOST</code> - JSON object of the crossposted item if the selected wallpaper is a crosspost</li>
    <li><code>WDOMAIN</code> - domain of the selected wallpaper</li>
    <li><code>WISGALLERY</code> - boolean value indicating whether the selected wallpaper is a gallery or not</li>
    <li><code>GITEM</code> - JSON object of a randomly selected item from the gallery if the selected wallpaper is a gallery</li>
    <li><code>WMIME</code> - MIME type of the selected wallpaper</li>
    <li><code>WEXT</code> - file extension of the selected wallpaper</li>
    <li><code>WID</code> - ID of the selected wallpaper</li>
    <li><code>WURI</code> - URL of the selected wallpaper</li>
    <li><code>WNAME</code> - filename of the selected wallpaper</li>
    <li><code>FILEPATH</code> - path to the downloaded wallpaper</li>
    <li><code>old_file</code> - path to the old desktop wallpaper</li>
    <li><code>new_file</code> - path to the new desktop wallpaper</li>
  </ul>
