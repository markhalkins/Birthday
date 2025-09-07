import { motion } from "framer-motion";

export default function BirthdayCake() { return ( <div className="flex flex-col items-center justify-center min-h-screen bg-gradient-to-b from-pink-200 to-yellow-100 p-4"> {/* Cake /} <div className="relative w-48 h-48"> {/ Bottom layer /} <motion.div initial={{ scaleY: 0 }} animate={{ scaleY: 1 }} transition={{ duration: 0.8, delay: 0 }} className="absolute bottom-0 w-48 h-16 bg-pink-400 rounded-t-lg shadow-lg" /> {/ Middle layer /} <motion.div initial={{ scaleY: 0 }} animate={{ scaleY: 1 }} transition={{ duration: 0.8, delay: 0.8 }} className="absolute bottom-16 w-40 h-12 bg-yellow-300 rounded-t-lg shadow-lg left-4" /> {/ Top layer /} <motion.div initial={{ scaleY: 0 }} animate={{ scaleY: 1 }} transition={{ duration: 0.8, delay: 1.6 }} className="absolute bottom-28 w-32 h-10 bg-white rounded-t-lg shadow-lg left-8" /> {/ Candle /} <motion.div initial={{ opacity: 0, y: -20 }} animate={{ opacity: 1, y: 0 }} transition={{ delay: 2.4 }} className="absolute bottom-40 left-1/2 -translate-x-1/2 w-2 h-8 bg-yellow-600 rounded" /> {/ Flame */} <motion.div initial={{ scale: 0 }} animate={{ scale: [1, 1.2, 1] }} transition={{ delay: 2.6, repeat: Infinity, duration: 0.6 }} className="absolute bottom-48 left-1/2 -translate-x-1/2 w-4 h-4 bg-orange-400 rounded-full shadow-md" /> </div>

{/* Texts */}
  <motion.h1
    initial={{ opacity: 0, y: 20 }}
    animate={{ opacity: 1, y: 0 }}
    transition={{ delay: 3 }}
    className="mt-12 text-3xl font-bold text-pink-700 drop-shadow-lg"
  >
    🎉 Happy Birthday 🎉
  </motion.h1>
  <motion.h2
    initial={{ opacity: 0, y: 20 }}

