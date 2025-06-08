import React from 'react';
import { Card, CardContent } from '@/components/ui/card';
import { Button } from '@/components/ui/button';

export default function TudoParaNamorados() {
  return (
    <div className="min-h-screen bg-pink-50 text-red-900">
      {/* Header */}
      <header className="bg-red-100 p-6 text-center shadow-md">
        <h1 className="text-4xl font-bold">TudoParaNamorados</h1>
        <p className="text-lg">Presentes românticos que dizem tudo ❤️</p>
      </header>

      {/* Página Inicial */}
      <section className="p-6">
        <h2 className="text-2xl font-semibold mb-4">Destaques da Semana</h2>
        <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
          <Card className="bg-white">
            <CardContent className="p-4">
              <img src="/cesta-romantica.jpg" alt="Cesta Romântica" className="rounded-xl mb-4" />
              <h3 className="text-xl font-bold">Cesta Amor Doce</h3>
              <p className="text-sm text-gray-600">Buquê, chocolates e pelúcia fofa.</p>
              <p className="text-lg font-bold mt-2">R$ 129,90</p>
              <Button className="mt-3 w-full">Comprar Agora</Button>
            </CardContent>
          </Card>
        </div>
      </section>

      {/* Página de Produto */}
      <section className="p-6 bg-white mt-8">
        <h2 className="text-2xl font-semibold mb-4">Detalhes do Produto</h2>
        <div className="grid grid-cols-1 md:grid-cols-2 gap-6">
          <img src="/cesta-romantica.jpg" alt="Produto" className="rounded-xl" />
          <div>
            <h3 className="text-xl font-bold mb-2">Cesta Amor Doce</h3>
            <p className="mb-2">Uma linda cesta com buquê, pelúcia (Stitch ou ursinho) e chocolates (Ferrero, BIS, Garoto, etc).</p>
            <p className="mb-2">Inclui embalagem romântica e laço decorativo.</p>
            <label className="block mb-2">Mensagem personalizada:</label>
            <textarea className="w-full p-2 border rounded-md mb-4" placeholder="Digite sua mensagem..." />
            <p className="text-lg font-bold mb-2">R$ 129,90</p>
            <Button>Adicionar ao Carrinho</Button>
          </div>
        </div>
      </section>

      {/* Página de Contato */}
      <section className="p-6 bg-red-50 mt-8 text-center">
        <h2 className="text-2xl font-semibold mb-4">Fale Conosco</h2>
        <p className="mb-2">Atendimento rápido e com carinho ❤️</p>
        <a
          href="https://wa.me/5599999999999"
          target="_blank"
          rel="noopener noreferrer"
          className="inline-block bg-green-500 text-white px-4 py-2 rounded-xl shadow hover:bg-green-600"
        >
          Falar no WhatsApp
        </a>
      </section>

      {/* Rodapé */}
      <footer className="text-center p-4 text-sm text-gray-600 mt-8">
        © 2025 TudoParaNamorados. Todos os direitos reservados.
      </footer>
    </div>
  );
}
