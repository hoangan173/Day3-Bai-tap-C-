# Day3-Bai-tap-C-
Bài tập nhập môn lập trình buổi 3
Giải phương trình bậc 2
{
            double a, b, c;
            Console.WriteLine("Nhap a: ");
            a = double.Parse(Console.ReadLine());
            Console.WriteLine("Nhap b: ");
            b = double.Parse(Console.ReadLine());
            Console.WriteLine("Nhap c: ");
            c = double.Parse(Console.ReadLine());
            Console.WriteLine($"Phuong Trinh bac hai: {a}x^2 + {b}x + {c} = 0");
            double d = b * b - 4 * a * c;
            if (d < 0)
            {
                Console.WriteLine("Phuong Trinh Vo Nghiem");
            }
            else if (d == 0)
            {
                Console.WriteLine($"Phuong Trinh co nghiem kep x = { -b / (2 * a)}");
            }
            else
            {
                double x1 = (-b + Math.Sqrt(d)) / (2 * a);
                double x2 = (-b - Math.Sqrt(d)) / (2 * a);
                Console.WriteLine($"Phuong Trinh co hai nghiem x = {x1} va x = {x2}");
            }
            Console.ReadLine();
        }
