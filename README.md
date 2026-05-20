# Solar Optimization Advisor Agent

An AI-powered multi-agent system that helps homeowners evaluate the feasibility and financial ROI of installing solar panels using real environmental data, live electricity pricing, and engineering-based calculations.

## Overview

The Solar Optimization Advisor simplifies the process of evaluating residential solar installations through natural language interaction.

Instead of manually researching solar irradiance, electricity tariffs, roof constraints, weather conditions, and financial calculations, users can describe their situation conversationally and receive a personalized solar feasibility report within minutes.

Example:

> “I’m in Delhi, I have a south-facing 10×6 meter roof with a 25° tilt, and I use about 850 kWh per month.”

The system automatically extracts technical parameters, retrieves environmental data, searches for local electricity rates, performs energy and ROI calculations, and generates a clear recommendation report.

## Problem Statement

Evaluating whether solar panels are financially worthwhile is often complicated and fragmented.

Homeowners typically need to:
- Research solar irradiance and weather conditions
- Understand roof orientation and tilt impact
- Estimate installation costs and panel efficiency
- Find accurate local electricity rates
- Calculate annual energy generation and ROI

Most available tools rely on static assumptions or generic calculators, making personalized decision-making difficult.

## Solution

The Solar Optimization Advisor automates the entire workflow using a modular multi-agent architecture.

The system:
- Extracts user inputs from natural language
- Retrieves weather and solar irradiance data
- Dynamically searches for local electricity pricing
- Calculates panel layout and annual energy generation
- Estimates savings and payback period
- Maintains conversational memory for multi-turn analysis

The result is a transparent and personalized solar feasibility assessment generated through a single interaction.

## Project Demo

Click the image below to watch the full walkthrough of the Solar Optimization Advisor Agent.

[![Solar Optimization Advisor Demo](https://img.youtube.com/vi/KAnArVnp5LY&t/maxresdefault.jpg)](https://www.youtube.com/watch?v=KAnArVnp5LY&t)

## Key Features

- Natural language parameter extraction
- Live electricity tariff search
- Solar irradiance and weather API integration
- Panel layout optimization
- Energy production estimation
- Financial ROI modeling
- Multi-turn conversational memory
- Human-readable recommendation reports

## Architecture

### 1. Input Extractor Agent
Converts user conversations into structured technical parameters such as:
- Roof dimensions
- Orientation and tilt
- Energy consumption
- Budget constraints

### 2. Data Collection Agent
Fetches environmental and geographic data including:
- Solar irradiance
- Temperature and weather patterns
- Latitude and longitude
- Cloud cover and efficiency-impacting conditions

### 3. Electricity Rate Search Agent
Performs live web searches to retrieve current residential electricity rates for the user's region.

Example:
> ₹8.2/kWh — Delhi Residential Electricity Tariff (2025)

This improves ROI accuracy and transparency.

### 4. Computation Agent

Runs deterministic engineering calculations for:
- Panel placement optimization
- Annual energy production
- System efficiency losses
- Cost estimation
- Financial payback analysis


### 5. Memory System

Maintains session context across conversations, allowing users to:
- Compare scenarios
- Modify assumptions
- Perform “what-if” analysis
- Continue discussions without restarting

### 6. Report Generator

Transforms technical outputs into a concise and understandable recommendation report containing:
- Recommended system size
- Estimated annual generation
- Savings projection
- Payback timeline
- Key assumptions and pricing sources

## Workflow

1. User provides requirements conversationally
2. Input extraction agent structures parameters
3. APIs fetch weather and irradiance data
4. Electricity pricing is retrieved dynamically
5. Computation engine performs solar and ROI calculations
6. Report generator creates personalized recommendations
7. Session memory stores context for future interaction

## Example Output

| Metric | Value |
|---|---|
| Recommended System Size | 5.4 kW |
| Estimated Annual Generation | 8,200 kWh |
| Estimated Annual Savings | ₹78,000 |
| Estimated Payback Period | 5.8 Years |


## Why Agentic AI?

Instead of relying on a fixed pipeline, the system uses specialized agents that independently handle:
- Parameter extraction
- External data retrieval
- Live pricing search
- Engineering computation
- Conversational memory

This enables adaptive multi-step reasoning and more natural user interaction.

## Tech Stack

### Core Technologies
- Python
- Jupyter Notebook / Kaggle

### LLM & AI
- Google Gemini API
- Prompt Engineering
- Multi-Agent Workflow Design

### APIs & Data Sources
- OpenWeather API
- Open-Meteo API
- REST APIs

### Backend & Utilities
- Requests
- Python Dotenv
- JSON Processing
- Regex Parsing
- Dataclasses

### System Design
- Sequential Agent Architecture
- Session Memory Management
- Tool Integration Patterns
- Engineering-Based Financial Modeling

## Future Improvements

- Satellite imagery-based roof analysis
- Battery storage optimization
- Dynamic utility plan comparison
- Installation company recommendation engine
- Real-time solar panel pricing integration
