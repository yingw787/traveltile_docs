---
date: 2016-03-09T20:08:11+01:00
title: Roadmap
weight: 20
---

This application's focus is on design and prototyping; several major features are needed before the application can be considered production-ready.

## User accounts/authentication

As of now, all created tiles are globally available, and anybody can edit any tile that is within the browser. Authentication using Facebook's Login API to create differentiated user accounts, and the subsequent display of tile subsets limited to the creator and his friend network, will dramatically improve the security, focus, and overall quality of this application.

## Mobile compatibility

This project was designed for Chrome on Desktop, and is not compatible with either iOS or Android. A port of this application for use on WebKit is highly desirable.

## Database Security

Current SQL queries are built with string concatenation. Future versions of this application will likely use a database ORM.

## Migration of Image Hosting from FileStack to AWS S3

The current FileStack solution has been unsatisfactory in terms of latency, cost, and scalability. S3 would offer similar benefits as FileStack, Cloudinary, or a similar image hosting service, but with dynamic pricing, better security, and higher uptime determined by an SLA.

## Google Maps markers

The Google Maps component supports the usage of markers; with this and relevant EXIF data from images in the photo album, a trace of the locations traveled to can be presented on the map, providing users with an understanding of the exact geographic locations of the trip.

## Contributing

This project is not maintained by me at the moment. If you would like to become the primary maintainer of this application, please fork the application and email me so I can redirect requests and update this webpage. Additionally, please feel free to submit a new [issue](https://github.com/yingw787/traveltile_opensrc/issues) if you happen to see a bug or a [pull request](https://github.com/yingw787/traveltile_opensrc/pulls) to suggest a new feature or patch.
