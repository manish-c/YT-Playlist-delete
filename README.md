# Youtube Playlist empty

To empty all the videos from your playlist.

## Running

Need to run below code in console while in editing mode of the playlist.

* Open the playlist you want to empty.
* Click on edit.
* Press \<F12>.
* Paste below code on console like shown in the screenshot.
* All the videos will be removed and the playlist will be empty.

```
var songs = $('body').getElementsByClassName("pl-video-edit-remove");

function emptyPlaylist(i) {
  setInterval(function() {
    songs[i].click();
  }, 200);

}

for (var i = 0; i < 1; ++i){
  emptyPlaylist(i);
}
```

setInterval(function () { document.querySelector('#primary button[aria-label="Action menu"]').click(); var things = document.evaluate( '//span[contains(text(),"Remove from")]', document, null, XPathResult.ORDERED_NODE_SNAPSHOT_TYPE, null ); for (var i = 0; i < things.snapshotLength; i++) { things.snapshotItem(i).click(); } }, 1000);
