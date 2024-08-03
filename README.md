- 👋 Hi, I’m @gunes60
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
gunes60/gunes60 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import math
points = [(1, 2), (3, 4), (5, 6), (7, 8)]

def euclideanDistance(point1, point2):
    x1, y1 = point1
    x2, y2 = point2
    return math.sqrt((x2 - x1)**2 + (y2 - y1)**2)
distances = []
for i in range(len(points)):
    for j in range(i + 1, len(points)):
        distance = euclideanDistance(points[i], points[j])
        distances.append(distance)
        
if distances:  
    min_distance = min(distances)
    print(f"Minimum mesafe: {min_distance}")
else:
    print("Mesafe hesaplanacak yeterli nokta yok.")
