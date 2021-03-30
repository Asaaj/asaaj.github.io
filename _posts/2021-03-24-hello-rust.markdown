---
layout: post
title:  "Hello, Rust"
date:   2021-03-24
categories: rust
---
# Hi, I'm Jacob

I figured I should finally start a blog. So, here it is.

First things first: a little about me. I am a C++ programmer by day, and I'm typically a C++ programmer by night, too. These days, however, I've been needing to change things up a bit. As much as I love C++ (which is a lot), 12 hours of it most days tends to be fairly mentally exhausting.

So in the interest of branching out, I (re-)started learning Rust. I played around with it a bit a year or so ago, but I got distracted by C++20. After going through some of the little projects I like to implement when learning a new language (like solving the [xkcd "Raptor" problem][xkcd-raptor] and implementing a basic CPU ray tracer), I have decided to try doing something big. After all, everyone seems to be talking about how Rust is the future of systems programming, right?

# Rusty Spoon

I've decided to work on a "basic" graphics engine using [Vulkan][vulkan-docs], which is a project I'm currently calling "Rusty Spoon". Specifically, I'm using [vulkano.rs][vulkano-home], a "safe Rust wrapper around the Vulkan API". I have never used Vulkan before, nor do I have much experience with GPU programming of any kind. This is going to be an endeavor.

And when I say it'll be a "basic" engine, I really just mean I have no idea how far I'll make it. Right now, I'm just working through tutorials from [vulkano.rs][vulkano-tutorial] and [vulkan-tutorial][vulkan-tutorial], learning about things like GLSL and Descriptor Sets.

Here's the current state of my project:

![Rusty Spoon v0.0.0.0.0.1](/assets/2021/03/rusty-spoon-v0.0.0.0.0.1.png)

So... it's in the early stages. I had the rectangle bouncing around like the Pong ball, but I scrapped that in my current effort to get it to spin in 3D (from the [introduction to descriptor sets in the Vulkan tutorial][vulkan-desc-pools]).

As with many things I've encountered so far in this project, I'm getting a little tripped up by how different vulkano.rs is from Vulkan. The concepts are all there, but the wrapper is much, much less explicit than Vulkan is so proud of being. That&mdash;combined with the relatively limited documentation in some areas, my own limited Rust knowledge, and the stark lack of practical examples of vulkano.rs on the internet&mdash;makes it relatively difficult to make progress in these early stages. So I'm currently trying to figure out Descriptor Sets.

So that's where I'm at now. I'm expecting that I'll have more interesting insights and things to talk about here in a little while when I am done with the tutorials and actually branching into my own content, but I just wanted to get myself writing for now.

[xkcd-raptor]: https://xkcd.com/135/
[vulkan-docs]: https://www.khronos.org/vulkan/
[vulkano-home]: https://vulkano.rs/
[vulkano-tutorial]: https://vulkano.rs/guide/introduction
[vulkan-tutorial]: https://vulkan-tutorial.com/
[vulkan-desc-pools]: https://vulkan-tutorial.com/en/Uniform_buffers/Descriptor_pool_and_sets
