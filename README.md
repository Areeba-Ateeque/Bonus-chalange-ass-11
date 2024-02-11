#Bonus chalange 
#assignment no:11
#1
sugar_level = int(input("Enter your sugar level: "))

if sugar_level > 100:
    print("Your sugar level is high.")
    print("You need to take medicine. Please consult your doctor.")
else:
    if sugar_level >= 90:
        print("Your sugar level is elevated.")
        print("You should consider managing your sugar intake, but no need for medicine at the moment.")
    else:
        print("Your sugar level is normal.")
        print("No need to eat medicine. Keep a balanced diet.")

#2:
# write a Python program that takes into account the daily routine of a 19-year-old girl who plays badminton for 3 hours every night and also studies. It prints messages based on the time spent on each activity:
total_hours_in_a_day = 24
study_hours_per_day = 6
badminton_hours_per_night = 3

remaining_study_hours = study_hours_per_day
remaining_free_hours = total_hours_in_a_day - badminton_hours_per_night - study_hours_per_day

print(f"Total hours in a day: {total_hours_in_a_day} hours")
print(f"Study hours per day: {study_hours_per_day} hours")
print(f"Badminton hours per night: {badminton_hours_per_night} hours\n")

# Check if there's enough time for study after playing badminton
if remaining_free_hours >= study_hours_per_day:
    print("The girl has enough time for studying after playing badminton.")
    remaining_study_hours = 0
else:
    print("The girl needs to manage her time more efficiently to ensure enough study hours after playing badminton.")
    remaining_study_hours -= remaining_free_hours

print(f"\nRemaining study hours: {remaining_study_hours} hours")


