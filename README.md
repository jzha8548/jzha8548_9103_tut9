# Quiz 8 

## Part 1：Imaging Technique Inspiration

I am inspired by slit-scan imaging, where a moving image is rebuilt from narrow slices captured at different moments. I want to use this time-displacement effect to make interaction feel like the canvas is recording and bending time rather than simply drawing shapes.

In this project, the user's movement or webcam input could be stretched into ribbons, delays, and fragmented traces. This technique fits the assignment because it connects visual form directly to time-based behaviour and creates a mechanic that feels interactive, experimental, and visually distinctive.

## Description

- **Inspiration:** Slit-scan imaging and time-based visual effects.
- **Goal:** Make the canvas behave like a temporal recorder, not just a drawing surface.
- **Effect:** User actions become delayed, stretched, and fragmented into visual ribbons.
- **Experience:** The result is an interactive visual language that feels like bending motion through time.

## For the Assignment

- It emphasizes **time-based behaviour** rather than static form.
- It creates a **unique interaction mechanic** that is both experimental and expressive.
- It allows the project to be **visually distinctive** while maintaining a clear connection to user input.

## Visual Reference

![Spiral staircase - time displacement inspiration](./images/Screenshot%202026-05-05%20at%2022.52.40.png)
*Figure 1. Spiral Slitscan. Image by Masakazu Matsumoto, published on Flickr on 27 March 2010. Source: [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Spiral_Slitscan;_March_2010.jpg), original Flickr source: [vitroids/4466430328](https://www.flickr.com/photos/vitroids/4466430328/).* 

![Second reference image for time displacement effect](./images/Screenshot%202026-05-05%20at%2022.53.09.png)
*Figure 2. Screenshot from **Slitscan Time Displacement Effect with p5.js**. Artwork by [Kristian Talley](https://github.com/kttalley), based on Daniel Shiffman’s [Coding Challenge #164: Slitscan Time Displacement Effect](https://thecodingtrain.com/challenges/164-slitscan/). Source: [Kristian Talley project page](https://design.kristiantalley.com/projects/hacktober23/slitscan-time-displacement-effect/).*


## Part 2: Coding Technique Exploration

### Coding Technique: Frame-History Slit-Scan using `createCapture()` and `copy()`

![Slit-scan coding technique screenshot](./images/Screenshot%202026-05-05%20at%2022.53.09.png)

*Figure 3. Screenshot of The Coding Train's **Slit-Scan Video** p5.js example, showing a live video image being rebuilt through copied vertical slices.*

**Example implementation and code:**

- [The Coding Train: Slit-Scan Video tutorial](https://thecodingtrain.com/tracks/pixels/pixels/slit-scan/)
- [p5.js Web Editor example code](https://editor.p5js.org/codingtrain/sketches/f_M7gry32)
- [Coding Challenge #164: Slitscan Time Displacement Effect](https://thecodingtrain.com/challenges/164-slitscan/)


### Discussion

A useful coding technique is a frame-history slit-scan system using `createCapture()` and `copy()`. The webcam frame is treated as source material; each frame, a narrow column or row is copied and stored, then older slices are redrawn across the canvas. This means the final image is built from many different moments instead of one live frame. It directly supports my imaging technique because motion becomes stretched, delayed, and fragmented. It can also become an interactive mechanic by changing slice direction, speed, or offset with mouse input.
