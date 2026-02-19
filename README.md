# yawp - yet another word processor

[![Hippocratic License HL3-CL-ECO-MY-SV-TAL-USTA-XUAR](https://img.shields.io/static/v1?label=Hippocratic%20License&message=HL3-CL-ECO-MY-SV-TAL-USTA-XUAR&labelColor=5e2751&color=bc8c3d)](https://firstdonoharm.dev/version/3/0/cl-eco-my-sv-tal-usta-xuar.html)

This is another one of raine's projects. As a disclaimer, I am an engineer, not a cs major, and I honestly don't really mess with web technologies very much. This software is (not done) and also experimental - so please don't use this for mission-critical applications, and if you do, please routinely export your data.

## So, what is this?

This project is designed to be an clean, efficient word processor that runs natively on your browser, with no cloud servers and stuff needed past the initial load (though some features can include it if you opt to use certain llms).

A lot of oss doesn't have too great of stuff in the way of spellcheck/grammar/etc, so the goal of that is to also bring it into this editor.

There's also going to be some (optional) llm assistance features. Think of it as an editor that tells you how bad your writing is instead of telling you how to write. Trying to thread the needle some on making something that's useful and doesn't contribute to brainrot but can also help people create better writing.

LLM assistance may need some external help - depending on your computer. Most models aren't light, so you usually have to use a cloud provider for that sorta stuff (or have a bunch of gpus or a M5 Pro Max Ultra Mega Mac Mini Studio with 1TB of memory). A lot of you chances are have decently powerful computers though already - you're on github so you're a bit technical (though I don't judge if you're running a 20 year old thinkpad - that's based af!) - so later hopefully I'll add a feature to run an llm with webgpu in your browser (there's some projects for that, not quite narrowed it down yet though what I'll use)

## How do I run this?

It's just a bun javascript application. Just run it with `bun run dev`. If you don't have bun, you can get it with `curl -fsSL https://bun.sh/install | bash`. Yes, I know piping to bash can be controversial (and you probably should'nt do it), but honestly that's the way most of you are going to do it (though I highly reccomend taking a look at the script first).

I am targeting linux at the moment, mostly because I just use linux, so I can't promise the build process on other os's. Chances are it will work, though more data is also needed.

Ideally once this is functional I'll host a version live at [https://yawp.raine.garden](https://yawp.raine.garden), as it's just a static page that I can dump it on a server or something of a sort.

## I thought you hated llm's for writing, why are you incorporating one into your projects?

LLMs (large language models, think ChatGPT, Gemini, or Claude), like any other tool, are just as they say - a tool. I don't believe that LLM's should be replacing your thought process - and that's why the intention of this is **to not have them write for you**. I could talk all day how LLM's should not be replacing human thought processes (for more info, this paper is a good (yet long) read [Your Brain on ChatGPT (arXiv preprint)](https://arxiv.org/pdf/2506.08872).

Instead, when enabled, which will be completely optional, think of them as an editor (that might not be as good as a real editor), but can instantly offer you feedback, point out minor mistakes, and such.

Research has shown that LLM's can be benificial as an editor of sorts, and one of the big defining features hinges on not having the AI really write for you (especially on the first draft). The goal of this project is to thread the needle of sorts - and make something that helps humans to write better with gentle parenting of sorts.

All of the research for this sorta stuff is very early, so I'm interested to see how this will go. If you have any interesting thoughts/research on this sorta stuff, feel free to use any stuff I make to test your hypothesis (and if you do! please let me know! you can contact me on my website at [https://raine.garden](https://raine.garden)).

## What's up with the license?

I've seen some open-source software used for some pretty bad stuff. And given the current state of the world, I don't want to be making software that enables some of that. I know surely someone could probably just run my code anyways if they aren't the best, but I want to give them a moment of pause at least hopefully of reflection.

Then again idk if anyone will ever use this except me, so who knows. The hippocratic license v3 seems like a safe bet though at the moment.

## I want to contribute

Wow, I didn't expect people to like my project that much! Or even read to the end of this readme. My writing is bad. I'm sorry about that.

Suggestions are welcome (just fork, branch, make a pr, you know a drill), as long as the code is good and it doesn't mess with the ethos of the project or make it unreliable for some users (i.e. don't make it only run on Windows 11 or have the llm actually changing the user text).

If you don't like that, the nice thing about open source software is you can just fork this distro and make your own text editor. That's a win-win for both of us! For those vibe coding with little human oversight out there, chances are this is you, and [here's a little guide how to do so](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo). Though I do suppose claude can also probably do it for you (or whatever model is good these days - I don't keep track of this sorta stuff).

Maybe later I'll make a contributors.md file (if anyone even contributes), though for the time being - just don't be a jerk.

## Did you write this readme with your word processor?

Not yet dogfooding - also because I haven't written the tool yet! If I do get it up and running - chances are I will!
