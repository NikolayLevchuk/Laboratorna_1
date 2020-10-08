# Laboratorna_1

//**********Variant_13

static void Main(string[] args)
        {
            string n,r;
            double P=0,a;
            do
            {
                Console.Write("Введите количество сторон правильного n-угольника ");
                n=Console.ReadLine();
            } while (Convert.ToInt32(n)<2 || 360 % Convert.ToInt32(n)!=0);
            Console.Write("Введите радиус ");
            r = Console.ReadLine();
            a = 2 * Convert.ToDouble(r) * Math.Tan(Math.PI / Convert.ToDouble(n));
            Console.WriteLine("Сторона "+n+"-угольника = "+a);
            P = Convert.ToDouble(n) * Convert.ToDouble(a);
            Console.WriteLine("Периметр правильного "+n+"-уголника = " + P);
        }
