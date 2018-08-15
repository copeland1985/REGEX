# REGEX
All of the unique Regular Expressions I develop for my projects.


# 1. VALID CANADIAN PHONE NUMBERS
Validates Canadian phone numbers only in following two formats '416-123-1234' or (416) 123-1234 with a valid 3-digit area code from the list of approved Canadian area codes.

^((\((204|226|236|249|250|289|306|343|365|367|403|416|418|431|437|438|450|506|514|519|548|579|581|581|581|581|587|604|613|639|647|672|705|709|778|780|782|807|819|825|867|873|879|902|905)\) ?)|((204|226|236|249|250|289|306|343|365|367|403|416|418|431|437|438|450|506|514|519|548|579|581|581|581|581|587|604|613|639|647|672|705|709|778|780|782|807|819|825|867|873|879|902|905)[-\s]))?\d{3}[-\s]\d{4}$

# 2. VALID BIRTH DATES
Validates a date to be in either YYYY-MM-DD, YYYY MM DD or YYYY\MM\DD format. Must have valid 4 digit year, 2 digit month 01-12, and valid 2 digit day of 01-31 or 0-30 depending on month and checks for February of 01-29.

^\d{4}[\-\/\s]?((((0[13578])|(1[02]))[\-\/\s]?(([0-2][0-9])|(3[01])))|(((0[469])|(11))[\-\/\s]?(([0-2][0-9])|(30)))|(02[\-\/\s]?[0-2][0-9]))$

# 3. VALID CANADIAN POSTAL CODE
Validates for 6 character Canadian postal code in L1L1L1 or L1L 1L1 format, not case sensitive, only allows valid first character from list.

^[ABCEGHJKLMNPRSTVXYabceghjklmnprstvxy]{1}\d{1}[A-Za-z]{1} *\d{1}[A-Za-z]{1}\d{1}$

# 4. VALID EMAIL ADDRESS
Validates standard email address format such as test@test.com and allows special characters.

^([a-zA-Z0-9_\-\.]+)*(\+[a-z0-9-]+)?@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.)|(([a-zA-Z0-9\-]+\.)+))([a-zA-Z]{2,4}|[0-9]{1,3})(\]?)$
