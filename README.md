# REGEX
All of the unique Regular Expressions I develop for my projects.


# 1. VALID CANADIAN PHONE NUMBERS
Validates Canadian phone numbers only in following two formats '416-123-1234' or (416) 123-1234 with a valid 3-digit area code from the list of approved Canadian area codes.

^((\((204|226|236|249|250|289|306|343|365|367|403|416|418|431|437|438|450|506|514|519|548|579|581|581|581|581|587|604|613|639|647|672|705|709|778|780|782|807|819|825|867|873|879|902|905)\) ?)|((204|226|236|249|250|289|306|343|365|367|403|416|418|431|437|438|450|506|514|519|548|579|581|581|581|581|587|604|613|639|647|672|705|709|778|780|782|807|819|825|867|873|879|902|905)[-\s]))?\d{3}[-\s]\d{4}$
