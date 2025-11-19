```
using System.Runtime.ConstrainedExecution;

namespace Program
{
    public interface IBuilder
    {
        public abstract void _initializeBuild();
        public abstract void _midBuild();
        public abstract void _finalizeBuild();
    }

    public class ProductBuilder : IBuilder
    {
        private Product _product = new Product();

        public Product GetProduct()
        {
            var result = _product;          // current product
            _product = new Product();       // reset
            return result;
        }

        public void _initializeBuild()
        {
            _product.Add("Initialized!");
        }

        public void _midBuild()
        {
            _product.Add("Middle Part Complete!");
        }

        public void _finalizeBuild()
        {
            _product.Add("Finalized!");
        }
    }

    public class Director
    {
        private IBuilder _builder;

        public Director(IBuilder builder)
        {
            this.Builder = builder;
        }

        public IBuilder Builder
        {
            set { _builder = value; }
        }

        public void BuildMinimalProduct()
        {
            _builder._initializeBuild();
        }

        public void BuildFullFeatureProduct()
        {
            _builder._initializeBuild();
            _builder._midBuild();
            _builder._finalizeBuild();
        }
    }

    public class Product
    {
        private List<string> _parts = new List<string>();

        public void Add(string value)
        {
            _parts.Add(value);
        }

        public override string ToString()
        {
            var final = "";
            _parts.ForEach(x => final += x + "\n");
            return final;
        }
    }

    public static class Program
    {
        public static void Main()
        {
            var _builder = new ProductBuilder();
            var _director = new Director(_builder);

            Console.WriteLine("Minimal Product:");
            _director.BuildMinimalProduct();
            Console.WriteLine(_builder.GetProduct().ToString());

            Console.WriteLine("Fully Featured Product:");
            _director.BuildFullFeatureProduct();
            Console.WriteLine(_builder.GetProduct().ToString());
        }
    }
}

```