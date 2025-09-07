# vm t-shirt sizing with k-means

author: anthony chambet — solution architect @ orange business  
date: 2025-05-06  
status: development phase — public  
license: provided as-is for research and prototype purposes only. all rights reserved by orange business for any production implementation or derivative work.

## purpose  
this notebook applies k-means clustering to real-world vm inventory data (extracted via rvtools and pre-filtered using a bash script).  
the clustering algorithm classifies each vm into a t-shirt size category (small, medium, large) according to cpu and ram allocation.  

## objective  
the objective is to provide a systematic, automated method for classifying workloads to support dynamic pricing models.  
this approach helps distinguish between:  

- committed capacity (minimum platform allocation, capex basis)  
- excess consumption (pay-as-you-go)  

such classification is relevant in hybrid infrastructure environments, where resources are provisioned as fixed capacity but usage fluctuates over time. the model supports continuous cost analysis without relying on cloud-native elasticity.  

## environment  
- jupyter notebook (containerized) or jupyterlite  
- data inputs currently based on rvtools exports (csv)  
- intended integration with external data sources for daily refresh and validation  

## end goal  
to integrate the model into an online tool that enables sales teams to:  

- generate trusted, up-to-date cost simulations  
- provide quotations based on dynamic vm sizing  
- align pricing with actual resource consumption patterns  
