```
namespace Program
{
    public interface ICar
    {
        string Drive();
    }

    public class Volkswagen : ICar
    {
        public string Drive()
        {
            return "vroom vroom but volkswagen";
        }
    }

    public class Audi : ICar
    {
        public string Drive()
        {
            return "vroom vroom but audi";
        }
    }

    public abstract class Factory
    {
        public abstract ICar CreateCar();

        public string UseCar(ICar car)
        {
            return car.Drive();
        }
    }

    public class VolkswagenFactory : Factory
    {
        public override ICar CreateCar()
        {
            return new Volkswagen();
        }
    }

    public class AudiFactory : Factory
    {
        public override ICar CreateCar()
        {
            return new Audi();
        }
    }

    public static class Program
    {
        public static void Main()
        {
            var vwFactory = new VolkswagenFactory();
            var audiFactory = new AudiFactory();
            
            UseFactory(vwFactory);
            UseFactory(audiFactory);
        }

        static void UseFactory(Factory factory)
        {
            var car = factory.CreateCar();
            Console.WriteLine(factory.UseCar(car));
        }
    }
}

```