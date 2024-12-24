# Python_Project
age_in_years = int(input("Enter your age in years: "))

unit = input("Enter your time unit (Months, Weeks, Days, Hours, Minutes, Seconds): ").lower()

# Define constants for better readability and maintainability
months_per_year = 12
weeks_per_year = 52
days_per_year = 365  # Note: This is an approximation, leap years are not considered
hours_per_day = 24
minutes_per_hour = 60
seconds_per_minute = 60

if unit == "months":
    age_in_months = age_in_years * months_per_year
    print(f"You have lived for approximately {age_in_months} months")

elif unit == "weeks":
    age_in_weeks = age_in_years * weeks_per_year
    print(f"You have lived for approximately {age_in_weeks} weeks")

elif unit == "days":
    age_in_days = age_in_years * days_per_year
    print(f"You have lived for approximately {age_in_days} days")

elif unit == "hours":
    age_in_hours = age_in_years * days_per_year * hours_per_day
    print(f"You have lived for approximately {age_in_hours} hours")

elif unit == "minutes":
    age_in_minutes = age_in_years * days_per_year * hours_per_day * minutes_per_hour
    print(f"You have lived for approximately {age_in_minutes} minutes")

elif unit == "seconds":
    age_in_seconds = age_in_years * days_per_year * hours_per_day * minutes_per_hour * seconds_per_minute
    print(f"You have lived for approximately {age_in_seconds} seconds")

else:
    print("Invalid time unit. Please enter 'months', 'weeks', 'days', 'hours', 'minutes', or 'seconds'.")
