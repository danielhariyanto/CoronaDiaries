# CoronaDiaries

## Inspiration
The COVID-19 pandemic presents an unprecedented challenge to humanity by mass-isolating individuals. While being cooped up in our rooms, awareness of our own mental health becomes more important than ever. Counselors, therapists, and "mental health" apps can be expensive and inaccessible to some, and so not many individuals are motivated to introspect and may unknowingly fall into mental health decline and moreover suffer from mental illnesses.

## What it does
Inspired to make personal mental health awareness more accessible, we built a user-friendly web app that motivates users to record "audio diaries". This app then runs a sentiment analysis of the diary entry using AWS Comprehend to output a "sentiment score", which indicates how positive/negative/neutral the user's entry was. Over time, these accumulated diary entries with their sentiment scores are able to show the user's general mood trends and establish a "mental health status" based on these data. The app is a safe place to store easy-to-record audio diaries and bring awareness to users of their mental health statuses over time.

## How we built it
The web app involves a front-end, which was made using React, and a back-end, which was made using Node. We used MongoDB as our database and used AWS S3 to store the audio diaries. We used AWS Transcribe to convert the audio in text and then used AWS Comprehend to run a sentiment analysis on the text. We used AWS Serverless to host our web app.