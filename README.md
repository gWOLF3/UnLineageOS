# UnLineage OS

AOSP (Android Open Source Project) is grossly huge. Its not easy to modify. Independent projects like lineage are cool, but still very difficult to navigate and customize since the AOSP is inherently huge and difficult to work with. 

Goal of this project is to break down and customize some LineageOS defaults. 

## LineageOS

- most popular, open source operating system.
- not tied to specific vendor
- good starting point to build off of
- good community (discord channel for asking questions)
- wiki helpful for building base version for different devices

## Understanding AOSP

> All referenced projects will be from my fork (openinternet-cc) - direct fork from LineageOS Repo. 

### Project Structure

Lineage uses `repo` command - see [here](https://source.android.com/setup/develop/repo) to read up on that. 

> Keep in mind that the AOSP is spread across many different git repositories. In this context, I am going to refer to the different relevant git repositories and how they relate to the whole. 

#### /android

https://github.com/openinternet-cc/android

This is meta repo, which gets used by Google's `repo` tool to generate the project structure. To a AOSP noob such as myself, this is actually really confusing at first and its not easy to understand exactly how its working. But the important part, is you can look at the xml manifest to get a glance at all the different git repos which are going to be included in your build. 

#### /android_frameworks_base

#### 

## Developing

- good resource guide for building more efficiently
http://blog.udinic.com/2014/07/24/aosp-part-3-developing-efficiently/ 



## Other Resources

- Udi Cohen blog - http://blog.udinic.com/2014/05/24/aosp-part-1-get-the-code-using-the-manifest-and-repo/



