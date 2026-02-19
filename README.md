# PetGreen-Market-
Alimentacion saludable y ecologica para mascotas 
import React, { useState } from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import { Textarea } from "@/components/ui/textarea";
import { Leaf, PawPrint, Recycle, ShoppingCart, MapPin } from "lucide-react";
import { motion } from "framer-motion";

export default function PetGreenMarket() {
  const [cartCount, setCartCount] = useState(0);

  const addToCart = () => {
    setCartCount(cartCount + 1);
  };

  return (
    <div className="min-h-screen bg-green-50 text-gray-800">
      {/* HERO SECTION */}
      <section className="text-center py-16 px-6 bg-green-600 text-white">
        <motion.h1
          initial={{ opacity: 0, y: -20 }}
          animate={{ opacity: 1, y: 0 }}
          transition={{ duration: 0.8 }}
          className="text-4xl md:text-5xl font-bold mb-4"
        >
          PetGreen Market S.A.S.
        </motion.h1>
        <p className="text-lg md:text-xl max-w-2xl mx-auto">
          Alimentación saludable y ecológica para mascotas en Bogotá, Colombia.
        </p>
        <div className="mt-6 flex justify-center items-center gap-4">
          <Button className="rounded-2xl text-lg px-6 py-3">Ver Productos</Button>
          <div className="flex items-center gap-2 text-lg">
            <ShoppingCart /> {cartCount}
          </div>
        </div>
      </section>

      {/* UBICACIÓN */}
      <section className="py-8 px-6 text-center bg-green-100">
        <h2 className="text-2xl font-semibold flex justify-center items-center gap-2">
          <MapPin /> Ubicación
        </h2>
        <p className="mt-2 text-lg">Bogotá D.C., Colombia</p>
      </section>

      {/* MISIÓN Y VISIÓN */}
      <section className="py-16 px-6 max-w-6xl mx-auto grid md:grid-cols-2 gap-8">
        <Card className="rounded-2xl shadow-lg">
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold mb-4 flex items-center gap-2">
              <PawPrint /> Misión
            </h2>
            <p>
              Somos una empresa dedicada a la comercialización de alimentos saludables y ecológicos para mascotas,
              ofreciendo productos naturales de alta calidad que contribuyen al bienestar animal y al cuidado del medio ambiente.
            </p>
          </CardContent>
        </Card>

        <Card className="rounded-2xl shadow-lg">
          <CardContent className="p-6">
            <h2 className="text-2xl font-semibold mb-4 flex items-center gap-2">
              <Leaf /> Visión
            </h2>
            <p>
              Para el año 2030, ser reconocidos en Bogotá como líderes en la comercialización de alimentos sostenibles
              para mascotas, destacándonos por nuestra innovación y compromiso ambiental.
            </p>
          </CardContent>
        </Card>
      </section>

      {/* PRODUCTOS CON PRECIOS */}
      <section className="py-16 px-6 bg-white">
        <h2 className="text-3xl font-bold text-center mb-12">Nuestros Productos</h2>
        <div className="grid md:grid-cols-2 lg:grid-cols-4 gap-6 max-w-6xl mx-auto">

          <Card className="rounded-2xl shadow-md">
            <CardContent className="p-6">
              <h3 className="text-xl font-semibold mb-2">Concentrado Orgánico</h3>
              <p>Alimento natural para perros libre de químicos artificiales.</p>
              <p className="font-bold mt-2">$85.000 COP</p>
              <Button className="mt-4 w-full" onClick={addToCart}>Agregar al carrito</Button>
            </CardContent>
          </Card>

          <Card className="rounded-2xl shadow-md">
            <CardContent className="p-6">
              <h3 className="text-xl font-semibold mb-2">Alimento Deshidratado</h3>
              <p>Comida natural para gatos conservada sin aditivos.</p>
              <p className="font-bold mt-2">$72.000 COP</p>
              <Button className="mt-4 w-full" onClick={addToCart}>Agregar al carrito</Button>
            </CardContent>
          </Card>

          <Card className="rounded-2xl shadow-md border-2 border-green-500">
            <CardContent className="p-6">
              <h3 className="text-xl font-semibold mb-2">Snacks Ecológicos ⭐</h3>
              <p>Producto innovador basado en economía circular.</p>
              <p className="font-bold mt-2">$25.000 COP</p>
              <Button className="mt-4 w-full" onClick={addToCart}>Agregar al carrito</Button>
            </CardContent>
          </Card>

          <Card className="rounded-2xl shadow-md">
            <CardContent className="p-6">
              <h3 className="text-xl font-semibold mb-2">Línea Premium</h3>
              <p>Alimento balanceado con empaque biodegradable.</p>
              <p className="font-bold mt-2">$110.000 COP</p>
              <Button className="mt-4 w-full" onClick={addToCart}>Agregar al carrito</Button>
            </CardContent>
          </Card>
        </div>
      </section>

      {/* OBJETIVOS */}
      <section className="py-16 px-6 bg-green-100">
        <h2 className="text-3xl font-bold text-center mb-8">Nuestros Objetivos</h2>
        <ul className="max-w-3xl mx-auto space-y-4 text-lg">
          <li className="flex items-start gap-2">
            <Recycle /> Implementar empaques biodegradables en la mayoría de nuestros productos.
          </li>
          <li className="flex items-start gap-2">
            <Recycle /> Trabajar con proveedores responsables y sostenibles.
          </li>
          <li className="flex items-start gap-2">
            <Recycle /> Desarrollar productos innovadores basados en economía circular.
          </li>
          <li className="flex items-start gap-2">
            <Recycle /> Promover el consumo responsable en Bogotá y Colombia.
          </li>
        </ul>
      </section>

      {/* FORMULARIO DE CONTACTO */}
      <section className="py-16 px-6 bg-white">
        <h2 className="text-3xl font-bold text-center mb-8">Contáctanos</h2>
        <div className="max-w-2xl mx-auto space-y-4">
          <Input placeholder="Nombre completo" />
          <Input placeholder="Correo electrónico" />
          <Textarea placeholder="Escribe tu mensaje aquí..." />
          <Button className="w-full">Enviar Mensaje</Button>
        </div>
      </section>

      {/* FOOTER */}
      <footer className="bg-green-700 text-white text-center py-6">
        <p>© 2026 PetGreen Market S.A.S. - Bogotá, Colombia</p>
      </footer>
    </div>
  );
}
