Title: Roadmap for Apache Infrastructure

This roadmap is not yet operational, we are testing things out.

`spu:fetch('https://cwiki.apache.org/confluence/plugins/viewsource/viewpagesrc.action?pageId=231116197')`

<script type="text/ecmascript">
// Change from local to external sources (fetched from cwiki)
// Browsers will automatically insert "file://" into the src when testing locally,
// so we crop that out as well while changing the source link.
const baseurl = location.protocol + "//" + location.hostname;
for (let element of document.querySelectorAll("link, img")) {
    if (element.href && element.href.match("/confluence/")) {
    	element.href = "https://cwiki.apache.org" + element.href.replace(baseurl, "");
    }
    if (element.src && element.src.match("/confluence/")) {
    	element.src = "https://cwiki.apache.org" + element.src.replace(baseurl, "");
    }
}
</script>



(This roadmap is fetched from our [cwiki roadmap page](https://cwiki.apache.org/confluence/display/INFRA/ASF+Infrastructure+Services+Roadmap).)
