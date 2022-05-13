# ClusteringDestinations
this notebook outlines how to create destination clusters for shipments relative to their distance to the origin and to the diameter of each cluster, this is particularly useful when consolidating

## Introduction

In this notebook we take a company's shipments information from its ERP, we first integrate data and clean up the information. The goal is to create destination clusters for consolidation purposes.

The steps are as follows:
1. Integrate the data and clean it up, especially the zip code information.
2. Convert the zip code information to latitude and longitude.
3. Create clusters by the relative distance of each zip code destination vs the origin. Each cluster has a different diameter, the farther the larger.
4. Calibrate the clusters for the average diameter to approximate the width constraint.
5. Abstract the cetroids (latitude and longitude) of the clusters to in turn append them to the shipment data along with the cluster number.

This project help identify where the destination clusters are to subsequently develop a consolidation workflow.

Associated projects: ShipmentsForecasting and LongHaulConsolidation
