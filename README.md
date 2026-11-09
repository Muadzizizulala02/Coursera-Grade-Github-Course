#!/bin/bash

# Simple Interest Calculator

# Get principal amount
echo "Enter the principal amount:"
read principal

# Get rate of interest
echo "Enter the rate of interest:"
read rate

# Get time period
echo "Enter the time period (years):"
read time

# Calculate simple interest
interest=$(echo "scale=2; ($principal * $rate * $time) / 100" | bc)

# Display result
echo "Simple Interest: $interest"
