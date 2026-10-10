# Multi-Tier Architecture Documentation

## Definition of Two-Tier Architecture
A Two-Tier Architecture is a software application design pattern where the application is split into two independent, communicating layers or tiers: the application/web tier and the database tier[span_3](start_span)[span_3](end_span).

## The Web/Application Tier
* **Role**: Serves the user interface, handles incoming HTTP requests from users, and manages web sessions[span_4](start_span)[span_4](end_span).

## The Database Tier
* **Role**: Responsible for storing persistent data, user credentials, and application metadata, as well as executing structured queries[span_5](start_span)[span_5](end_span).

## Why Separate Them?
Separating the web server and the database into two distinct containers rather than packing them both into a single container provides better modularity, easier scaling, and independent maintenance[span_6](start_span)[span_6](end_span). If one tier experiences heavy traffic or requires an update, it can be managed or scaled independently without crashing or disrupting the entire application stack[span_7](start_span)[span_7](end_span).

