import java.util.Scanner;

public class RealQuadraticSolver {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.println("Solve ax^2 + bx + c = 0 (real roots only)");
        System.out.print("Enter a: ");
        double a = sc.nextDouble();
        System.out.print("Enter b: ");
        double b = sc.nextDouble();
        System.out.print("Enter c: ");
        double c = sc.nextDouble();

        if (a == 0.0) {
            if (b == 0.0) {
                if (c == 0.0) {
                    System.out.println("Infinite solutions (0 = 0).");
                } else {
                    System.out.println("No solution (constant nonzero).");
                }
            } else {
                double x = -c / b;
                System.out.printf("Linear equation. Single real root: x = %.6f%n", x);
            }
        } else {
            double discriminant = b * b - 4.0 * a * c;

            if (discriminant < 0.0) {
                System.out.println("No real roots (discriminant < 0).");
            } else if (discriminant == 0.0) {
                double x = -b / (2.0 * a);
                System.out.printf("One real root (double): x = %.6f%n", x);
            } else {
                double sqrtD = Math.sqrt(discriminant);
                double x1 = (-b + sqrtD) / (2.0 * a);
                double x2 = (-b - sqrtD) / (2.0 * a);
                System.out.printf("Two real roots: x1 = %.6f, x2 = %.6f%n", x1, x2);
            }
        }

        sc.close();
    }
}
