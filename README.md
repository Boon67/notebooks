# External File Download to Snowflake Stage

This notebook demonstrates an end-to-end setup and configuration for downloading files from external public URLs directly into a Snowflake internal stage using Python libraries within a Snowpark environment. It also includes a Streamlit application for a user-friendly interface to manage these downloads.

## Table of Contents

- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Setup and Configuration](#setup-and-configuration)
  - [Step 1: Create Internal Stage and Event Table](#step-1-create-internal-stage-and-event-table)
  - [Step 2: External Network Rules and Access Integration](#step-2-external-network-rules-and-access-integration)
- [File Download Logic](#file-download-logic)
- [Streamlit File Management Application](#streamlit-file-management-application)
- [Cleanup](#cleanup)

## Overview

The primary goal of this demonstration is to showcase how Snowflake's external access capabilities can be leveraged to retrieve data from external sources and store it within Snowflake for further processing. This involves:
- Setting up necessary Snowflake objects (stage, event table).
- Configuring network rules and external access integrations for secure external communication.
- Implementing Python code to download files from a URL.
- Providing a Streamlit interface for interactive file management on the stage.

## Prerequisites

Before running this notebook, ensure you have:
- A Snowflake account.
- Sufficient privileges (ACCOUNTADMIN for initial setup, SYSADMIN for ongoing operations).
- A Snowpark environment set up for running Python code within Snowflake.
- Familiarity with SQL and Python.