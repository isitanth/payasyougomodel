 Author: Anthony Chambet [Solution Architect @ Orange Business] – 2025/05/06
Under Dev phase.
# Purpose:
This notebook processes real-world VM inventory data (extracted via RVTools and pre-filtered using a Bash script)
and applies K-Means clustering to dynamically classify each VM into a T-shirt size category (Small, Medium, Large)
based on its CPU and RAM allocation.

# Objective:
The goal is to enable a scientific and automated classification mechanism to support dynamic pricing models,
distinguishing between minimum platform commitments and Pay-As-You-Go (PAYG) excess consumption.
This approach is relevant in hybrid infrastructure contexts where resources are provisioned as fixed-capacity (CAPEX),
but usage fluctuates over time. It allows for continuous-time cost modeling without relying on cloud-native elasticity.

# Environment
Jupyter Notebook (containerized) or JupyterLite. Both works properly.
The end goal is to use it within an online tool and fetch other data sources around to make the tool trusted and updated on a daily basis, while empowering a simple easy way to make quotation and simulation for sales teams.
