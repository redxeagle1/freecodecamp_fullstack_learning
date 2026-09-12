# Media Handling

- The `<audio>` and `<video>` elements allow you to add sound and video content to your HTML documents.
- The `<audio>` element supports popular audio formats like mp3, wav, and ogg.
- The `<video>` element supports mp4, ogg, and webm formats.

## The `<audio>` Element

the `<audio>` come with attribute to control its behavior common ones are:

- `src` To include your audio media via **file path** or a **url** but it will not display the media in the page
  - an example will be `<audio src="https://cdn.freecodecamp.org/curriculum/js-music-player/cruising-for-a-musing.mp3"></audio>`
- `controls` attribute is a **boolean attribute** which will show us audio player of the current given media

    ```html
    <audio 
        src="https://cdn.freecodecamp.org/curriculum/js-music-player/cruising-for-a-musing.mp3"
        controls
    ></audio>
    ```

  > Note: Some browsers, such as Safari, may not display a volume control by default even when the controls attribute is present.

- `loop` attribute is a **boolean attribute** that makes the audio replay continuously

    ```html
    <audio 
        src="https://cdn.freecodecamp.org/curriculum/js-music-player/cruising-for-a-musing.mp3"
        controls
        loop
    ></audio>
    ```

- `muted` attribute is a **boolean attribute** which will start the audio in a muted state

    ```html
    <audio
        src="<https://cdn.freecodecamp.org/curriculum/js-music-player/can't-stay-down.mp3>"
        loop
        controls
        muted
    ></audio>
    ```

### Supporting multiple media formats

- When it comes to audio file types, there are differences in which browsers support which type.
- To accommodate such differences, use `<source>` elements inside the `<audio>` element and **the browser will select the first source that it understands**.

    ```html
        <audio
            loop
            controls
            muted
        >
            <source src="audio.ogg" type="audio/ogg" />
            <source src="audio.wav" type="audio/wav" />
            <source src="audio.mp3" type="audio/mpeg" />
        </audio>
    ```

## The `<video>` Element

the `<video>` element support the same attribute of `<audio>` element but adds the following upon that:

- `autoplay` attribute is a boolean attribute which will start video automatically
- `width` attribute defines the video size making it bigger or smaller

    ```html
    <video
        src="https://archive.org/download/BigBuckBunny_124/Content/big_buck_bunny_720p_surround.mp4"
        loop
        controls
        muted
        autoplay
        width="400"
    ></video>
    ```

- `poster` attribute to display an image while the video is downloading, and take image path as a value

### Supporting multiple video formats

You can also use the source element inside a video element, just like you did with the audio element. This lets you provide the same video in multiple formats, and the browser will choose the first one it can play.

```html
<video
    controls
    width="400"
    poster="https://peach.blender.org/wp-content/uploads/title_anouncement.jpg?x11217"
>
    <source
        src="https://archive.org/download/BigBuckBunny_124/Content/big_buck_bunny_720p_surround.mp4"
        type="video/mp4"
    />
    <source
        src="https://archive.org/download/BigBuckBunny_124/Content/big_buck_bunny_720p_surround.webm"
        type="video/webm"
    />
    Your browser does not support the video tag.
</video>
```
