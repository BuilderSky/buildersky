## Hello, Folks!!! This is BuilderSky here!
### You may also know me as Sky777 from numerous other places, or perhaps *E4C* (*Engines 4 Christ*) from YouTube!!!

I do enjoy many different things, including lots of computer stuff, but I love fiddling with vehicles the most!!! That's why I created a YouTube channel, Engines 4 Christ, to document my journey through reviving two 1974 DJ Postal Jeeps! You can actually view [my channel](https://www.youtube.com/channel/UCeY5jNrEbLARbo-1ddJfVew "E4C on YouTube") here! ;)

And, of course, if you don't want to have to view my channel, here is my latest*** video:
<p>

<div style="text-align:center;">
<a style="align:center" href="http://www.youtube.com/watch?feature=player_embedded&v=B_4o8rvX6yE" target="_blank"><img src="http://img.youtube.com/vi/B_4o8rvX6yE/0.jpg" 
alt="YouTube Video" width="600" height="425" />
</a>
</div>

const requestOptions = {
    method: 'GET',
    redirect: 'follow'
};

const loadVideo = (iframe) => {
    const cid = iframe.getAttribute('cid');
    const channelURL = encodeURIComponent(`https://www.youtube.com/feeds/videos.xml?channel_id=${cid}`)
    const reqURL = `https://api.rss2json.com/v1/api.json?rss_url=${channelURL}`;
    fetch(reqURL, requestOptions)
        .then(response => response.json())
        .then(result => {
            const videoNumber = (iframe.getAttribute('vnum') ? Number(iframe.getAttribute('vnum')) : 0);
            const link = result.items[videoNumber].link;
            const id = link.substr(link.indexOf("=") + 1);
            iframe.setAttribute("src", `https://youtube.com/embed/${id}?controls=0&autoplay=1`);
        })
        .catch(error => console.log('error', error));
}
var iframes = document.getElementsByClassName('latestVideoEmbed');
for (var i = 0, len = iframes.length; i < len; i++) {
    loadVideo(iframes[i]);
}

██████████████████████████████████████████████
█░░░░░░░░░░░░░░█░░░░░░██░░░░░░█░░░░░░░░░░░░░░█
█░░▄▀▄▀▄▀▄▀▄▀░░█░░▄▀░░██░░▄▀░░█░░▄▀▄▀▄▀▄▀▄▀░░█
█░░▄▀░░░░░░░░░░█░░▄▀░░██░░▄▀░░█░░▄▀░░░░░░░░░░█
█░░▄▀░░█████████░░▄▀░░██░░▄▀░░█░░▄▀░░█████████
█░░▄▀░░░░░░░░░░█░░▄▀░░░░░░▄▀░░█░░▄▀░░█████████
█░░▄▀▄▀▄▀▄▀▄▀░░█░░▄▀▄▀▄▀▄▀▄▀░░█░░▄▀░░█████████
█░░▄▀░░░░░░░░░░█░░░░░░░░░░▄▀░░█░░▄▀░░█████████
█░░▄▀░░█████████████████░░▄▀░░█░░▄▀░░█████████
█░░▄▀░░░░░░░░░░█████████░░▄▀░░█░░▄▀░░░░░░░░░░█
█░░▄▀▄▀▄▀▄▀▄▀░░█████████░░▄▀░░█░░▄▀▄▀▄▀▄▀▄▀░░█
█░░░░░░░░░░░░░░█████████░░░░░░█░░░░░░░░░░░░░░█
██████████████████████████████████████████████

I would love it if you would view my [GitHub progress](https://skyline.github.com/BuilderSky/2022) for this year, too! ;) 

### ***Currently being manually updated, may not be the latest video!