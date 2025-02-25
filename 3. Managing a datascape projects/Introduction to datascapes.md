---
title: Introduction to datascapes
layout: home
nav_order: 1
parent: Managing Datascape Projects
---
# Introduction to datascapes
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

1. what is a datascape
	1. components
	2. features
2. import/open a datascape
3. creating datascapes (manually from interface, from files, or programmatically)
4. designing a datascape (workflow)


# What is a datascape: components and complexity

A datascape is the visual environment where you interact with your data as it is the data and media files composing it. 

In its most basic form, a datascape only requires a single node file. But it also will use a tag file to manage the tags in the scene, images, 3D objects.

What is a datascape :
- 3D objects and models
	- primitives geometries
- data in csv format
- images textures
- tags files

Minimum viable datascape: a node file is all it takes to display 

## Supported file formats

GaiaViz will load the following formats:
- Image files: `tiff`,`jpg`,`png`
- 3D models files: 
- Video streams: `YUV`, `RGB`

# Basic datascapes editing : "WYSIWYG"

- direct creation of your datascape allow to 
- geometry, colors

## Manually create from the interface


A datascape is a folder on your local file system where GaiaViz stores your data.
The most elementary form is a node.csv file, and the most complex datascapes includes images, tags files, 3D models, plugins, animation track.

You can keep all your datascapes in one place, or create several folders for each of your different projects.


- Create a manual datascape: 
	Open GaiaViz app and start create one in app

- Open existing datascape: If you have a datascape that you wish to open:
	1. Open GaiaViz and hit the "L" keyboard key to open the Load Dialog
	2. Navigate to your datascape location and select the .bat file
Saving a datascape from the app will generate a .bat file.
To import a datascape, hit the "L" key, navigate the file dialog to the 

- Create a datascape programmatically


# Advanced datascapes: Python
Advanced datascapes may contain animation (using the channel and tracks methods), pipe live data from external sensors and 
## Programmatically with data tools
# Designing a datascape : workflow per user type
1- ideas, mock-up and asset collection
2- assets wrangling and iteration
3- clean-up, bundle and share

## Data analysts
Data analysts' typical workflow will involve a lot of data mani

## Graphic and motion designer

# Manage datascapes
