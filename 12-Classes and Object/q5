
class Time:
    def __init__(self, hours=0, minutes=0, seconds=0):
        self.hours = hours
        self.minutes = minutes
        self.seconds = seconds
        self.normalize()

    def normalize(self):
        self.minutes += self.seconds // 60
        self.seconds %= 60
        self.hours += self.minutes // 60
        self.minutes %= 60

    def __str__(self):
        return f"{self.hours:02}:{self.minutes:02}:{self.seconds:02}"

    def __add__(self, other):
        new_hours = self.hours + other.hours
        new_minutes = self.minutes + other.minutes
        new_seconds = self.seconds + other.seconds
        return Time(new_hours, new_minutes, new_seconds)

    def __sub__(self, other):
        total_self = self.to_seconds()
        total_other = other.to_seconds()
        total_diff = abs(total_self - total_other)
        return Time.from_seconds(total_diff)

    def to_seconds(self):
        return self.hours * 3600 + self.minutes * 60 + self.seconds

    def from_seconds(seconds):
        hours = seconds // 3600
        seconds %= 3600
        minutes = seconds // 60
        seconds %= 60
        return Time(hours, minutes, seconds)

time1 = Time(2, 45, 50)
time2 = Time(1, 20, 30)

print("Time 1:", time1)
print("Time 2:", time2)

sum_time = time1 + time2
print("Time 1 + Time 2:", sum_time)

diff_time = time1 - time2
print("Time 1 - Time 2:", diff_time)

print("Time 1 in seconds:", time1.to_seconds())
print("Time 2 in seconds:", time2.to_seconds())
