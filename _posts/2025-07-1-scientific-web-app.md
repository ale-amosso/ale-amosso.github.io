---
layout: post
title: "Scientific Web App"
date: 2025-07-11
tags: [python, react, setup]
author: Alessandra Amosso
---

## Scientific Web App
Some days ago I was talking with my friend Lucia, who is an expert in Bayesian Inference, about creating an audio denoise project together, since she is recording conferences sometimes and the output sometimes is not that listenable. But then I wondered "how should we do it? A Python script? A web service?". But since I don't like to keep thigs simple, I have decided to drag her in the creation of a React Web App, with a Python back-end. So, let's start with the passages we have faced. 

## Step 1 — Create your project folder with a virtual environment

Since I am always very scared about installing packages in my computer that could end up destroying other projects because of conflicts, the first step is always to create a virtual environment.
After having created the project folder with a backend folder and a frontend folder, open the command prompt e launch this for creating the virual environment

```bash
cd backend
python -m venv venv
```
## Step 3 — Activate the virtual environment

On Windows:
```bash
.\venv\Scripts\activate
```

The backend will be structured as follow: controller that "talks" with the GUI and the core of the project: the DENOISERRR. 
## Step 4 — Install packages for FastAPI
We have decided to use FastAPI for the controller to talk with the GUI, hence, in the backend folder we have to install.

```bash
pip install fastapi uvicorn python-multipart
```

FastAPI is a modern web framework for building APIs with Python.
Uvicorn is an ASGI web server implementation for Python.
Multipart is a library for uploading files (more or less).



## Step 5 — Frontend
Dowload and Install Node.js from the https://nodejs.org/en/download, preferabily the Long term version
Go to the frontend folder and check that it is installed correctly
```bash
node -v
npm -v
```
Then create the React Project with Vite
```bash
npm create vite@latest
```
It will ask you to choose the name of the project, write just a dot "." for creating the project without a new name, inside the current folder.
Then it will ask you the type 


```bash
Project name: › .
```
Then choose the React framework


```bash
> React
```
and finally the variant Javascript because we don't hate ourselves enough to choose Typescript

```bash
> Javascript
```

Then it will ask you to do:


```bash
  npm install
  npm run dev
```

Then it will tell you which is the port that we should use, open your preferred browser and paste the link there, you should have something like this:

<figure>
  <img src="/assets/images/11_07_25/react_page.png" alt="Starting interface" width="800">
  <figcaption>Fig. 1: Starting React page. </figcaption>
</figure>

## Step 6 — Create the homepage


The starting point of the interface is the file
```bash

frontend/src/App.jsx 
```





That’s it!
Good luck with your new project :)

