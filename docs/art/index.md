Got a cool sticker design for your hack that you want to shared? Submit a PR [here](https://github.com/Hackathons-UK/hexbin) and get it on display here!

Thinking about getting one? [Check here for more info](/organise/before/stash_and_swag)

Please share it as a vector (SVG, EPS, etc)!
<style>
#stickerframe {
    width: 100%;
    min-width: 100%;
    position: relative;
}
</style>

<iframe src="/art/hexbin/stickers.html" frameborder="0" id="stickerframe" scrolling="no" style="border: none; width: 100%" ></iframe>

<script type="text/javascript" src="https://cdnjs.cloudflare.com/ajax/libs/iframe-resizer/4.2.8/iframeResizer.min.js"></script>

<script>

    var loadHexes = function() {

		var stickerFrame = document.getElementById("stickerframe");
		
		var onStickerFrameLoad = function() {

			stickerFrame.removeEventListener("load", onStickerFrameLoad);

			iFrameResize({heightCalculationMethod: "lowestElement"});
			stickerFrame.contentWindow.location.reload();
		};

    	stickerFrame.addEventListener("load", onStickerFrameLoad);

	}

    if(document.readyState === "complete") {

    	loadHexes();

	} else {

		document.addEventListener("DOMContentLoaded", loadHexes);

	}

</script>
