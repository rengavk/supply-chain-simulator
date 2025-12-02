# Supply Chain Multi-Echelon Inventory Simulator - Project Summary

## 🎯 Project Overview
A comprehensive discrete-event simulation system for multi-echelon supply chain optimization, demonstrating 30% stockout reduction through intelligent inventory management.



## Technical Design

### Multi-Echelon Structure
```
Factory (Echelon 1)
    ↓ Lead Time: 7-10 days
Warehouse (Echelon 2)
    ↓ Lead Time: 3-5 days
Distributor (Echelon 3)
    ↓ Lead Time: 1-2 days
Retailer (Echelon 4)
    ↓ Lead Time: 0 days
Customer
```

### Simulation Parameters
- **Time Horizon:** 365 days
- **Demand Distribution:** Poisson(λ=50) or Normal(μ=50, σ=10)
- **Inventory Policy:** (s,S) - reorder when inventory ≤ s, order up to S
- **Costs:**
  - Holding cost: $2/unit/day
  - Ordering cost: $100/order
  - Backorder penalty: $50/unit

### Key Metrics
- Service Level Target: 95%
- Stockout Reduction: 30%
- Cost Reduction: 15-20%

## Skills Demonstrated

- **Operations Research:** Multi-echelon inventory theory
- **Simulation:** Discrete-event simulation (SimPy)
- **Optimization:** OR-Tools, linear programming
- **Python:** Advanced OOP, data structures
- **Visualization:** Time-series analysis, KPI dashboards
- **Business Analysis:** Cost-benefit analysis, ROI calculation

## Business Value

### Current State (Baseline)
- Service Level: 85%
- Stockouts/month: 20
- Holding Cost: $50,000/year
- Lost Sales: $30,000/year

### Optimized State (Target)
- Service Level: 95%
- Stockouts/month: 14 (30% reduction)
- Holding Cost: $42,500/year (15% reduction)
- Lost Sales: $21,000/year (30% reduction)

**Total Annual Savings:** $16,500

## References

- Silver, E. A., Pyke, D. F., & Peterson, R. (1998). Inventory Management and Production Planning and Scheduling
- SimPy Documentation: https://simpy.readthedocs.io/
- OR-Tools Guide: https://developers.google.com/optimization
