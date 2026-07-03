# Frequently Asked Questions

## Installation & Compatibility

**Q: Is this cable compatible with my NVIDIA/Mellanox system?**
A: This cable works with NVIDIA Quantum-2 switches (400G OSFP) and ConnectX-6/X6 adapters (200G QSFP56). It's compatible with DGX A100/H100 systems, HPE and Dell GPU servers. Check the compatibility matrix in technical-specs.md.

**Q: Does my switch firmware need updating?**
A: Latest firmware supporting active optical is required. All modern versions (released 2023+) support active optical cables. Adapter firmware should also be latest version.

**Q: Can I hot-swap this cable?**
A: Yes, these cables are hot-swappable. No power-down required for replacement.

## Technical Questions

**Q: Why active optical instead of passive DAC?**
A: At 3 meters, passive DAC cables degrade significantly and require external signal conditioning equipment. Active optical maintains full 400Gbps integrity while consuming only 10-12W of power.

**Q: What's the power consumption?**
A: Typical operation: 10-12W. Peak startup: 15W. Idle: 0.5-1.0W. This is minimal compared to passive alternatives requiring 25W+ conditioning equipment.

**Q: How does this cable handle power budgets in dense racks?**
A: With only 10-12W per cable, even 20+ cables consume minimal power (240W total). This fits within standard data center power and thermal budgets.

**Q: Can I use shorter cables?**
A: Yes, but they limit architectural flexibility. The 3m length is optimized for standard rack spacing. Shorter cables (1-2m) force denser configurations that may cause thermal issues.

**Q: Can I use longer cables?**
A: Longer cables (>3m) are possible but introduce latency and heat in dense racks. For longer distances, consider adding additional switch tiers instead.

## Deployment & Operations

**Q: How many cables do I need for my deployment?**
A: For each 400G OSFP port you want to connect to 2x200G QSFP56, you need 1 cable. For redundancy, multiply by 2. Reference deployment-scenarios.md for typical configurations.

**Q: What's the lead time for ordering?**
A: Standard stock items ship within 2-3 days. Bulk orders (50+ cables) may require 1-2 weeks for aggregate fulfillment.

**Q: Do you offer custom lengths?**
A: Yes, 2m, 5m, and 10m variants available for enterprise deployments. Contact sales for custom length quotes.

**Q: What's the warranty?**
A: 5-year manufacturer warranty from shipment date. Lifetime technical support during business hours.

## Performance & Troubleshooting

**Q: What latency does this cable add?**
A: Total end-to-end latency is ~15 nanoseconds (negligible for data center applications). This includes ~10.5ns optical path + ~2-3ns active electronics.

**Q: How do I test if the cable is working?**
A: Modern switches report optical power levels for each cable. Use management interface to verify received power (-11 dBm typical). Cables also auto-shutdown if signal degrades.

**Q: What if I see signal degradation?**
A: Check for: (1) Bent fibers/physical damage, (2) Connector cleanliness, (3) Cable temperature (<50°C under load), (4) Firmware version match between switch and adapter.

**Q: Can temperature variations affect performance?**
A: Operating range is 0-70°C. At these temperatures, performance is unaffected. Auto-shutdown occurs at >85°C as a safety feature.

## Cost & ROI

**Q: How does total cost compare to alternatives?**
A: 3m AOC cables + zero conditioning equipment = lower total cost than passive DAC + signal conditioning. Annual cooling savings for 50-rack deployment: $50,000+.

**Q: Is this investment future-proof?**
A: Yes. 400G OSFP and 200G QSFP56 are finalized standards. These cables will remain relevant for 5+ years as GPU technology evolves around these standards.

**Q: What about lifecycle and replacement?**
A: MTBF (Mean Time Between Failures) >50 years. In practice, cables outlast the systems they connect. Most data center upgrades replace cabling due to architecture changes, not failures.

## Standards & Compliance

**Q: What standards does this cable meet?**
A: IBTA HDR, IEEE 802.3 400G, OSFP/QSFP56 MSA, CMIS 5.0, RoHS, REACH. Fully MSA-compliant with vendor-neutral design.

**Q: Is this cable laser-safe?**
A: Yes, Class 1 laser product. Safe for human exposure in normal conditions.

**Q: Can I use this in data centers outside the US?**
A: Yes, RoHS and REACH compliant for EU, ISED compliant for Canada. Check local regulations for your specific region.

## Support & Returns

**Q: How do I get technical support?**
A: Email: support@... or phone during business hours. RMA process for defective units typically completed within 5 business days.

**Q: What's your return policy?**
A: 30-day return window for unopened/unused cables. Warranty covers manufacturing defects for 5 years from shipment.
