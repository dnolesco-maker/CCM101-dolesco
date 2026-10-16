# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A two-tier architecture is a system design that separates an application into two main parts: the web/application tier and the database tier. These two tiers communicate with each other to process requests and manage data.

## The Web/Application Tier

The web/application tier is responsible for displaying the user interface and handling HTTP requests from users. In this mission, Nextcloud serves as the web application that allows users to access and manage their files through a browser.

## The Database Tier

The database tier stores and manages persistent data, such as user account information and file metadata. In this mission, MariaDB serves as the database that Nextcloud connects to when it needs to store or retrieve information.

## Why Separate Them?

Separating the web application and database into two containers makes the system easier to manage and maintain. Each container has its own responsibility, so the web application and database can be configured or updated independently. This separation also makes it easier to troubleshoot problems in one component without rebuilding the entire application.
