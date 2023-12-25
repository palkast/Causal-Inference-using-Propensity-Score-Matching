# Causal-Inference-using-Propensity-Score-Matching
This notebook is created to explain the use of Propensity Score Matching to infer causality in situations where it is not logically possible to randomize.PSM is used to reduce the bias due to confounding variables that could be found in an estimate of treatment effect obtained from simply comparing outcomes among the teratement and control groups.


Propensity Score Matching
Model treatment as a function of observed variables 
(Use Logit/Probit to do this)
Get predicted probabilities of treatment from the model

For each treated observation, find control observation with closest predicted probabilities (up to a specified threshold aka caliper) 
If no match found, remove observation from analysis


What Problems Do You See Here?

Omitted Variable Bias – Still don’t know what we don’t know. PSM assumes that treatment is determined by observed variables 
Lack of Support – There may not be any good matches. Choice of caliper is somewhat arbitrary 
Propensity Function – Logit or Probit is just as arbitrary as conditioning on the controls linearly! 



