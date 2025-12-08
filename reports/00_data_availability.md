📄 00_data_availability.md
Data Availability & Analytical Scope
Objective

The purpose of this project is to analyze player movement and interaction during the ball-in-air window of passing plays. This report documents what data is available, how the “ball in the air” period is defined, and what types of analysis this dataset enables — and does not enable.

Dataset Overview

We use the NFL Big Data Bowl input, output, and supplementary datasets, which together provide tracking and contextual information for passing plays.

Input data
Player tracking before the ball is thrown.

Output data
Player tracking after the ball is thrown, from release to outcome.

Supplementary data
Play-level contextual data including pass result and game situation.

Importantly, the tracking data does not include explicit event markers such as pass_forward or pass_arrived.

Defining the “Ball-in-Air” Window

The dataset defines the “ball-in-air” phase implicitly:

The transition from the final frame of input data to the first frame of output data corresponds to the moment the ball is thrown.

All frames in the output tracking files correspond to player movement while the ball is in flight.

The final output frame corresponds to the play outcome (catch, incompletion, or interception), which is labeled in the supplementary data.

This implicit structure allows us to precisely isolate and analyze post-throw player behavior, without relying on noisy or missing event labels.

Spatial & Temporal Resolution

Player positions are recorded as (x, y) coordinates in yards.

Frame frequency is approximately 10 Hz (0.1 seconds per frame).

Player identities (nfl_id) are consistent across frames and files.

No direct kinematic variables (speed, acceleration, heading) are provided.

What This Data Enables

✅ Enabled analyses:

Separation dynamics during ball flight

Defender reaction speed and pursuit efficiency

Receiver–defender interaction patterns

Degree of contest at the catch point

❌ Not enabled:

Quarterback decision-making analysis

Route development before the throw

True three-dimensional ball trajectory modeling

Summary

This dataset supports a focused, high-resolution analysis of player movement after the throw — the most decisive window in passing outcomes. All metrics in this project are intentionally scoped to that window.
