import React from "react"; import { Card, CardContent } from "@/components/ui/card"; import { Button } from "@/components/ui/button"; import { motion } from "framer-motion";

export default function HomePage() { return ( <div className="min-h-screen bg-black text-white px-6 py-10"> <motion.h1 initial={{ opacity: 0, y: -20 }} animate={{ opacity: 1, y: 0 }} transition={{ duration: 0.5 }} className="text-4xl font-bold text-center mb-10 text-blue-500" > Formulaire de Demande </motion.h1>

<motion.div
    initial={{ opacity: 0, y: 20 }}
    animate={{ opacity: 1, y: 0 }}
    transition={{ duration: 0.5 }}
    className="max-w-2xl mx-auto bg-gray-800 p-6 rounded-2xl shadow-md"
  >
    <form className="grid grid-cols-1 gap-4">
      <input type="text" placeholder="Nom" className="p-3 rounded bg-gray-700 text-white" required />
      <input type="text" placeholder="Prénoms" className="p-3 rounded bg-gray-700 text-white" required />
      <input type="text" placeholder="Profession" className="p-3 rounded bg-gray-700 text-white" required />
      <input type="number" placeholder="Âge" className="p-3 rounded bg-gray-700 text-white" required />
      <input type="text" placeholder="Ville" className="p-3 rounded bg-gray-700 text-white" required />
      <input type="text" placeholder="Objet de la demande" className="p-3 rounded bg-gray-700 text-white" required />
      <input type="number" placeholder="Somme demandée (€)" className="p-3 rounded bg-gray-700 text-white" required />
      <input type="tel" placeholder="Numéro de téléphone" className="p-3 rounded bg-gray-700 text-white" required />
      <Button type="submit" className="bg-blue-600 hover:bg-blue-700 mt-4">Soumettre</Button>
    </form>
  </motion.div>
</div>

); }


