# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A Two-Tier Architecture is a system where the application is divided into two main parts: the Web/Application Tier and the Database Tier. The Web/Application Tier handles the requests from the users, while the Database Tier stores and manages the information used by the application.

## The Web/Application Tier

The Web/Application Tier is the part of the system that users interact with. It displays the application interface, receives HTTP requests, processes user actions, and communicates with the database. In this project, **Nextcloud** is used as the Web/Application Tier.

## The Database Tier

The Database Tier stores and manages the application's data. It can contain user accounts, passwords, file information, and other data needed by the application. In this project, **MariaDB** is used as the Database Tier.

## Why Separate Them?

It is better to place the web application and database in separate containers because each service has its own purpose and can be managed independently. If one container needs to be updated or restarted, the other container does not have to be changed. This also makes the system easier to maintain and scale.
