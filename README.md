import math

def calculate_area_circle(radius):
    return math.pi * radius**2

def calculate_area_rectangle(length, width):
    return length * width

def calculate_area_triangle(base, height):
    return 0.5 * base * height

def main():
    while True:
        print("\nSelect a shape to calculate the area:")
        print("1. Circle")
        print("2. Rectangle")
        print("3. Triangle")
        print("4. Exit")

        choice = input("Enter your choice (1-4): ")

        if choice == '1':
            radius = float(input("Enter the radius of the circle: "))
            area = calculate_area_circle(radius)
            print(f"The area of the circle is: {area}")
        elif choice == '2':
            length = float(input("Enter the length of the rectangle: "))
            width = float(input("Enter the width of the rectangle: "))
            area = calculate_area_rectangle(length, width)
            print(f"The area of the rectangle is: {area}")
        elif choice == '3':
            base = float(input("Enter the base of the triangle: "))
            height = float(input("Enter the height of the triangle: "))
            area = calculate_area_triangle(base, height)
            print(f"The area of the triangle is: {area}")
        elif choice == '4':
            print("Exiting the program.")
            break
        else:
            print("Invalid input. Please enter a number between 1 and 4.")

if __name__ == "__main__":
    main()
