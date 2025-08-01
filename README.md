## READ ME

# This script generates Spatial BioCondition training datasets by generating a pool of sites from various sources, scoring them against benchmarks, and then
# assesses each site against a series of auditing criteria. Spatial datasets are available via QSpatial or TERN data portal.This workflow has several parts:

# 1) Workspace setup: creates the project directory structure and loads required libraries
# 2) Site summaries: imports and processes raw tabular data from QBEIS and QBERD to generate site summaries of BioCondition attributes
# 3) Site compiler: compiles all site summaries into a single training data pool with standardised formatting and data structure
# 4) RE assignment: checks site REs against the latest version of REDD, and changes/assigns conflicts via RE mapping, landzone  and composition data
# 5) Site scoring: scores sites against the latest version of benchmarks (including drafts), and assigns a score to each site where possible
# 6) Site assessment: assesses sites against a series of spatial criteria to ensure they meet the requirements for inclusion in the training dataset
# 7) Site auditing: selects sites based on the scoring and assessment criteria, and generates a final training dataset
