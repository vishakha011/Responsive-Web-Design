# Responsive Web Design

With the growth in mobile Internet usage comes the question of how to build websites suitable for all users. Mobile devices can’t be ignored as more and more people rely on them to access the web. The industry response to this question has become responsive web design, also known as RWD. 

## Why RWD?
- Your website looks great of the desktop screen but it may not be true when your site is viewed on a smartphone or a tablet. Once you make the design responsive, the website will look good (and readable) on all screens.
- With Responsive Design you can create one design and it will automatically adapt itself based on the screen size of the mobile device. This approach offers plenty of advantages:
- It saves time and money as you don’t have to maintain separate websites for desktops and mobile phones.
- Responsive Design is good for your website’s SEO (search rankings) as every page on your site will have a single URL. You don’t have to worry about situations where some sites link to your mobile site while others link to your desktop site.
- Your Google Analytics reports will paint a better picture of your site’s usage since the data from mobile and desktop users will be consolidated.
- Responsive Designs are easier to maintain as they do not involve any server-side components. You just have to modify the underlying CSS of a page to change its appearance (or layout) on a particular device.

## What is Responsive Web Design?
Responsive web design is a method or an approach where a designer creates a web page which resizes itself according to the type of device it is seen through. In this method, development and design respond based on the user’s behavior and environment. The practice consists of a mix of images, flexible grids, and layouts and a smart use of CSS media queries. As the user moves from their laptop to iPhone, the website should immediately switch to accommodate for image size, resolution and scripting abilities.

Basically, the website should have the technology to respond, automatically to the user’s preferences. This removes the need to design and develop differently for each new gadget on the market.

Responsive web design is broken down into three main components, 
flexible layouts

1. Media Queries
2. Flexible Media. 
3. Flexible Layouts

### Flexible layouts 
It is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width.
Flexible grids are built using relative length units, most commonly **percentages** or **em** units. These relative lengths are then used to declare common grid property values such as width, margin, or padding.

Flexible layouts do not advocate the use of fixed measurement units, such as pixels or inches. The reason being, the viewport height, and width continually change from device to device.

### Media Queries
Media queries were built as an extension to media types commonly found when targeting and including styles. Media queries provide the ability to specify different styles for individual browser and device circumstances, the width of the viewport or device orientation for example. Being able to apply uniquely targeted styles opens up a world of opportunity and leverage to responsive web design.
```
@media all and (min-width: 800px) and (max-width: 1024px) {...}
@media not screen and (color) {...}
@media only screen and (orientation: portrait) {...}
```
**Media feature in media Queries:-**

- Height & Width Media Features
- Orientation Media Feature
- Aspect Ratio Media Features
- Resolution Media Feature etc.

**Width :** Describes the width of the targeted display area of the output device. This is a range value, which means that you can also use min-width and max-width.

**Height :** Describes the height of the targeted display area of the output device. This is a range value, which means that you can also use max-width.

**Orientation :** Describes the orientation of the device. It is portrait when the value of the height media feature is greater than or equal to the value of the width media feature.

**Aspect Ratio :** The ratio of the value of the width media feature to the value of the height media feature.

**Resolution :** Describes the resolution of the output device (i.e. the density of the pixels).

### Flexible media
This part deals with making all media contents responsive. It can adjust to what ever the screen size it is used on. Images and videos are made to response in accordance with width of the media device screen and orientation. This also includes about embeded media to make responsive. Although max-width property does not work in all types of media.

## Identifying break points:-
There are certain common breakpoints of viewport sizes as determined by different device resolution such as 320px, 480px, 768px, 1024px, 1224px . But taking this point commonly in use is not a good idea. Instead, it must be defined in accordance with the working of the web layout. It must be introduced only when a website starts to break, look weird or the experience is being hampered.
Responsive layouts are made in mainly two approaches.
1. Mobile first
2. Desktop first

**Mobile First :-**
This approach is made to make a web layout in keeping mind about the screen size of the mobile and then a media query is applied to make it responsive. Applying media query to get it adjusted in all media devices be it desktop or tablet etc.

**Viewport :-**
On the other hand in desktop-first approach the styles are first applied to desktop or larger devices. Thereafter advanced styles are written to override the styles for small screen devices via media query.

Generally, the layout for larger devices is a bit complicated than the smaller devices. And loading desktop styles on smaller viewport devices would be a bad idea. Most of the time default we can rely on default properties of elements for smaller screens.

    It is believed that taking a mobile-first approach is considered as best practice, and it's true also. Although you can take any approach that depends upon personal choice. But the mobile-first approach has some advantages over the desktop-first approach.


## Viewport :
A Browser’s viewport is the area of a web page in which the content is visible to the user. The viewport does not have the same size, it varies with the variation in screen size of the devices on which the website is visible. For a laptop, the viewport has a larger size as compared to a smartphone or tablet.
The common setting of the viewport is —
```
<meta name=”viewport” content= “width=device-width, initial-scale=1.0”>
```
**content=width=device-width :** it sets viewport to a special value(“width= device-width”) which is the width of the device in terms of CSS pixels at a scale of 100%

**initial-scale :** initial-scale property governs the zoom level when the page is loaded for the first time.
