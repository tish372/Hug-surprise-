import { useState } from "react"; import { Button } from "@/components/ui/button"; import { Card, CardContent } from "@/components/ui/card"; import { motion } from "framer-motion";

const messages = [ "Hey you!", "Click me!", "Just one more...", "Almost there!", "Here it comes...", ];

export default function CuteSurprise() { const [step, setStep] = useState(0);

const handleClick = () => { if (step < messages.length) { setStep(step + 1); } };

return ( <div className="flex flex-col items-center justify-center min-h-screen bg-pink-100 p-4"> {step < messages.length ? ( <motion.div key={step} initial={{ scale: 0.8, opacity: 0 }} animate={{ scale: 1, opacity: 1 }} transition={{ duration: 0.5 }} className="mb-6" > <Card className="rounded-2xl shadow-xl p-6 bg-yellow-100 border-yellow-300"> <CardContent className="text-center text-lg font-semibold text-pink

# Hug-surprise-
