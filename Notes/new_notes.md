# Full Stack Development Notes

## HTML Basics

- You can add audio and video elements to an HTML page using `audio` and `video`

## Links and External Resources

- The target attribute on anchor / link elements determine where the page opens; \_self = current browsing context; \_blank = new context (e.g. new tab); \_parent = in parent of the current context; \_top = top-most context
- Links can have five different states: `:link`, the default (unclicked) state; `:visited`;`:hover`; `:focus` when the link is focused using Tab; `:active` when clicked; the order listed here is also the order that must be specified in CSS

## Audio and Video

- The `audio` element can have different attributes that control how it behaves: `src` for providing the audio file, `loop` to control if the audio loops (`loop` is a bool and doesn’t need a value)
- The `controls` attribute in `audio` is also a bool that provides the user with controls to play/stop the media file.
- The `video` element has a `width` attribute
- The `video` element also has the bool attributes `loop` and `controls`
- Both `audio` and `video` elements have the `muted` attribute, to control if the media is muted when the first playback starts

## Video Formats

- When it comes to `video` format support, it is browser dependent; so you need to provide multiple types of video, that the browser can select. The syntax is:

```html
  <source src="src-url-goes-here" type="video-type-goes-here" />
```

- Media types must be specified using a MIME format (ex. `video/mp4`)
- All the popular video format types are: `video/mp4` `video/webm` `video/ogg` and `video/quicktime`

## Iframes

- iframes are replaced elements; replaced elements are elements whose contents are determined by an external source, rather than CSS (e.g. website, image, embedded video)
- iframe can also be used to embed another HTML page directly
- When embedding a video, the `allow` attribute defines an allowlist of features that the embedded content is allowed to use (e.g. autoplay, accelerometer, clipboard-write)

## Media Considerations

- When using media, you should consider: size, format and compression\

## Images

- Image formats for older browsers: PNG, JPEG; more modern formats: WEBP, AVIF
- Images on the web are by default released under “All Rights Reserved”; use tools like Unsplash/Pixabay to find images with permissive licenses

## SVG

- SVGs are vector graphics, and they can be defined directly in HTML; they are useful when wanting to have custom icons on your page, e.g. for social media icons
- SVG stores the data in XML format
