# Define the input variables (all in pesos)
landscape_area_cost = 1000000 # Cost over the landscape area
ecosystem_services_cost = 500000 # Potential ecosystem services cost
remediation_cost = 2000000 # Remediation cost over the affected area at risk
treatment_cancer_cost = 1500000 # Cost of treatment of cancer over the populations at risk
treatment_non_cancer_cost = 800000 # Cost of treatment of non-cancer diseases over the
populations at risk
mining_proceeds = 5000000 # Capital (monetary benefits) generated from mining proceeds
# Model formula: Net Benefit = Mining Proceeds - Total Costs
net_benefit = mining_proceeds - (landscape_area_cost + ecosystem_services_cost +
 remediation_cost + treatment_cancer_cost +
treatment_non_cancer_cost)
# Decision rule
if net_benefit > 0:
 decision = "Mine"
else:
 decision = "Do Not Mine"
# Display results
print(f"Net Benefit: {net_benefit} pesos")
print(f"Decision: {decision}")
