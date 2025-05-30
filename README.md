// VORTIX — موقع مصغر

import React from 'react';
import { Card, CardContent } from '@/components/ui/card';
import { Button } from '@/components/ui/button';
import { Sparkles, Crown, Users, LogIn, LayoutDashboard, MessageCircle } from 'lucide-react';
import { motion } from 'framer-motion';

export default function Home() {
  return (
    <div className="min-h-screen bg-gradient-to-br from-blue-950 to-blue-900 text-white p-6">
      <motion.h1
        initial={{ opacity: 0, y: -30 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ duration: 0.8 }}
        className="text-4xl md:text-6xl font-bold text-center mb-6 text-blue-200 drop-shadow-lg"
      >
        ✦ تم افتتاح خادم VORTIX ✦
      </motion.h1>

      <motion.div
        initial={{ opacity: 0 }}
        animate={{ opacity: 1 }}
        transition={{ delay: 0.5, duration: 0.8 }}
        className="grid md:grid-cols-3 gap-6"
      >
        <Card className="bg-blue-950/60 backdrop-blur border border-blue-600 shadow-xl">
          <CardContent className="p-4 space-y-3">
            <h2 className="text-xl font-semibold flex items-center gap-2 text-blue-100">
              <Crown className="text-yellow-400" size={20}/> الرتب
            </h2>
            <ul className="list-disc ml-6 text-blue-200">
              <li>✦ founder - 𓆩𖤐𓆪</li>
              <li>✿ co-owner - 𖦹</li>
              <li>✧ head admin - ⟡</li>
              <li>⋯ والمزيد</li>
            </ul>
          </CardContent>
        </Card>

        <Card className="bg-blue-950/60 backdrop-blur border border-blue-600 shadow-xl">
          <CardContent className="p-4 space-y-3">
            <h2 className="text-xl font-semibold flex items-center gap-2 text-blue-100">
              <LayoutDashboard className="text-green-400" size={20}/> أهم الغرف
            </h2>
            <ul className="list-disc ml-6 text-blue-200">
              <li>V・🎀・roles・𖠌</li>
              <li>V・🕷️・rules・人</li>
              <li>V・💬・general-chat・彡</li>
              <li>V・🎁・giveaways・ト</li>
              <li>⋯ والمزيد</li>
            </ul>
          </CardContent>
        </Card>

        <Card className="bg-blue-950/60 backdrop-blur border border-blue-600 shadow-xl">
          <CardContent className="p-4 space-y-3">
            <h2 className="text-xl font-semibold flex items-center gap-2 text-blue-100">
              <Users className="text-pink-400" size={20}/> الرُتب التفاعلية
            </h2>
            <ul className="list-disc ml-6 text-blue-200">
              <li>⟡ member - ˖</li>
              <li>✿ active - ❁</li>
              <li>✺ engaged - ☽</li>
              <li>✧ community pillar - ⊹</li>
              <li>⋯ وهكذا</li>
            </ul>
          </CardContent>
        </Card>
      </motion.div>

      <motion.div
        initial={{ opacity: 0, y: 20 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ delay: 1.2, duration: 0.8 }}
        className="mt-12 text-center"
      >
        <p className="text-blue-200 mb-4 text-lg">انضم إلينا وكن جزءًا من تجربة خيالية ✧</p>
        <Button className="bg-gradient-to-r from-purple-700 to-blue-600 shadow-xl hover:scale-105 transition">
          <LogIn className="mr-2" size={18}/> دعوة إلى الخادم
        </Button>
      </motion.div>

      <motion.div
        initial={{ opacity: 0, y: 20 }}
        animate={{ opacity: 1, y: 0 }}
        transition={{ delay: 1.5, duration: 0.8 }}
        className="mt-16 text-center text-sm text-blue-400"
      >
        ⛧ VORTIX COMMUNITY © 2025 — تم التطوير بحب من أجلكم
      </motion.div>
    </div>
  );
}
