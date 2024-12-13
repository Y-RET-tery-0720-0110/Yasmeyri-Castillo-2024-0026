# Yasmeyri-Castillo-2024-0026
Creacion clase cliente
C:\Users\HP-PC\source\repos\TAREA 8 EN GIT HUB\TAREA 8 EN GIT HUB\CLIENTE completado.cs
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace TAREA_8_EN_GIT_HUB
{
    public class CLIENTE 
    {
        private List<PEDIDO> historialCompra = new List<PEDIDO>();

        public int Id { get; set; }
        public string Nombre { get; set; }
        public string Apellido { get; set; }
        public string Direccion { get; set; }
        public string CorreoElectronico { get; set; }
        public List<PEDIDO> HistorialCompra { get => historialCompra; set => historialCompra = value; }
        public CLIENTE(List<PEDIDO> historialCompra)
        {
            HistorialCompra = historialCompra;
        }

        public CLIENTE()
        {
        }

        public CARRITO CARRITO { get; set; } = new CARRITO();

        public void RealizarCompra(PRODUCTO pantalon)
        {
            Console.WriteLine("comprar pantalon jean");
        }
        public void AgregarProducto(PRODUCTO pRODUCTO)
        {
            throw new NotImplementedException();
        }

        public List<PRODUCTO> Productos { get; set; } = new List<PRODUCTO>();
        public double Total { get; set; }

        public void Agregar(PRODUCTO producto)
        {
            producto.Add(producto);
            Total += producto.Precio;
        }
        public void RemoverProducto(PRODUCTO producto)
        {
            Console.WriteLine("error durante el pago");
        }

    }
}

