```aura width=860 height=200
 <div style={{
 width: '100%', height: '100%', background: '#08080c',
 display: 'flex', alignItems: 'center', fontFamily: 'Inter',
 position: 'relative', overflow: 'hidden', borderRadius: 16,
 border: '1px solid rgba(110,80,220,0.18)'
}}>

 <style>
   {`
     @keyframes float-slow {
       0%, 100% { transform: translateX(0px); opacity: 0.8; }
       50% { transform: translateX(350px); opacity: 1.2; }
     }
     @keyframes float-medium {
       0%, 100% { transform: translateX(0px); opacity: 0.7; }
       50% { transform: translateX(-250px); opacity: 1.1; }
     }
     @keyframes float-fast {
       0%, 100% { transform: translateX(0px); opacity: 0.9; }
       50% { transform: translateX(200px); opacity: 0.6; }
     }
     @keyframes float-diagonal {
       0%, 100% { transform: translateX(0px); opacity: 0.75; }
       50% { transform: translateX(300px); opacity: 1.0; }
     }
     @keyframes float-wave {
       0%, 100% { transform: translateX(0px); opacity: 0.65; }
       33% { transform: translateX(-160px); opacity: 0.9; }
       66% { transform: translateX(80px); opacity: 1.0; }
     }
     @keyframes float-pulse {
       0%, 100% { transform: scale(1); opacity: 0.8; }
       50% { transform: scale(1.3); opacity: 0.4; }
     }
     #glow-1 { animation: float-slow 8s ease-in-out infinite; }
     #glow-2 { animation: float-medium 12s ease-in-out infinite; }
     #glow-3 { animation: float-fast 9s ease-in-out infinite; }
     #glow-4 { animation: float-slow 11s ease-in-out infinite reverse; }
     #glow-5 { animation: float-medium 14s ease-in-out infinite reverse; }
     #glow-6 { animation: float-diagonal 10s ease-in-out infinite; }
     #glow-7 { animation: float-wave 13s ease-in-out infinite; }
     #glow-8 { animation: float-pulse 7s ease-in-out infinite; }
   `}
 </style>

 <svg width="860" height="200" style={{ position: 'absolute', top: 0, left: 0 }}>
   <defs>
     <radialGradient id="g1" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(110,20,210,0.72)" />
       <stop offset="40%" stopColor="rgba(90,15,180,0.35)" />
       <stop offset="70%" stopColor="rgba(90,15,180,0)" />
     </radialGradient>
     <radialGradient id="g2" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(40,60,255,0.6)" />
       <stop offset="45%" stopColor="rgba(30,50,200,0.25)" />
       <stop offset="70%" stopColor="rgba(30,50,200,0)" />
     </radialGradient>
     <radialGradient id="g3" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(0,130,255,0.45)" />
       <stop offset="50%" stopColor="rgba(0,100,220,0.18)" />
       <stop offset="70%" stopColor="rgba(0,100,220,0)" />
     </radialGradient>
     <radialGradient id="g4" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(0,190,230,0.32)" />
       <stop offset="70%" stopColor="rgba(0,190,230,0)" />
     </radialGradient>
     <radialGradient id="g5" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(90,30,200,0.38)" />
       <stop offset="70%" stopColor="rgba(90,30,200,0)" />
     </radialGradient>
     <radialGradient id="g6" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(160,30,255,0.55)" />
       <stop offset="45%" stopColor="rgba(130,20,220,0.22)" />
       <stop offset="70%" stopColor="rgba(130,20,220,0)" />
     </radialGradient>
     <radialGradient id="g7" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(20,60,255,0.42)" />
       <stop offset="50%" stopColor="rgba(10,40,200,0.16)" />
       <stop offset="70%" stopColor="rgba(10,40,200,0)" />
     </radialGradient>
     <radialGradient id="g8" cx="50%" cy="50%" r="50%">
       <stop offset="0%" stopColor="rgba(0,170,255,0.40)" />
       <stop offset="50%" stopColor="rgba(0,130,220,0.15)" />
       <stop offset="70%" stopColor="rgba(0,130,220,0)" />
     </radialGradient>
   </defs>

   <ellipse id="glow-1" cx="180" cy="230" rx="260" ry="190" fill="url(#g1)" />
   <ellipse id="glow-2" cx="300" cy="240" rx="220" ry="160" fill="url(#g2)" />
   <ellipse id="glow-3" cx="420" cy="240" rx="180" ry="140" fill="url(#g3)" />
   <ellipse id="glow-4" cx="550" cy="250" rx="150" ry="120" fill="url(#g4)" />
   <ellipse id="glow-5" cx="750" cy="250" rx="130" ry="110" fill="url(#g5)" />
   <ellipse id="glow-6" cx="300" cy="240" rx="180" ry="140" fill="url(#g6)" />
   <ellipse id="glow-7" cx="490" cy="230" rx="220" ry="170" fill="url(#g7)" />
   <ellipse id="glow-8" cx="590" cy="250" rx="150" ry="130" fill="url(#g8)" />
 </svg>

 <div style={{
   position: 'absolute', left: 48, top: 52, width: 96, height: 96,
   borderRadius: 48, background: 'linear-gradient(135deg, #6622ee, #0088ff)',
   display: 'flex', alignItems: 'center', justifyContent: 'center',
 }}>
   <img src=".github/assets/avatar.png" width={88} height={88} style={{ borderRadius: 44, objectFit: 'cover' }} />
 </div>

 <div style={{ display:'flex', flexDirection:'column', marginLeft:168, gap:8, zIndex: 10 }}>
   <div style={{ display:'flex', fontSize:38, fontWeight:800, color:'#ffffff', letterSpacing:'-1px', lineHeight:1 }}>
     Adam Khan
   </div>
   <div style={{ display:'flex', fontSize:15, color:'rgba(180,165,255,0.8)', fontWeight:400, letterSpacing:'0.3px' }}>
     I build stuff. | Agents, LLMs & applied AI
   </div>
   <div style={{ display:'flex', gap:8, marginTop:6 }}>
     {['Python', 'TypeScript', 'LangGraph', 'TensorFlow'].map(function(tag) {
       return (
         <div key={tag} style={{
           display:'flex', padding:'4px 12px', borderRadius:20,
           background:'rgba(80,40,220,0.18)', border:'1px solid rgba(100,70,240,0.32)',
           color:'rgba(205,195,255,0.85)', fontSize:12, fontWeight:600,
         }}>{tag}</div>
       );
     })}
   </div>
 </div>
</div>
```

```aura width=860 height=140
(function() {
 // Graph totals: 284 (2024) + 533 (2025) + 252 (2026). readme-aura only exposes owned-repo commits (~75).
 var graphContributions = 284 + 533 + 252;
 var apiCommits = (github && github.stats && github.stats.totalCommits) || 0;
 var bigNumber = Math.max(graphContributions, apiCommits);
 // Matches tech stack pills below (5 + 6 + 6).
 var stackCount = 17;
 var stats = [
   { label: 'Repos', value: String((github && github.stats && github.stats.totalRepos) || 0), color: '#a78bfa' },
   { label: 'Contributions', value: String(bigNumber), color: '#60a5fa' },
   { label: 'Stack', value: String(stackCount), color: '#f59e0b' },
 ];

 return (
   <div style={{
     width: '100%', height: '100%',
     background: '#08080c',
     display: 'flex', alignItems: 'center', justifyContent: 'center',
     fontFamily: 'Inter', borderRadius: 16,
     border: '1px solid rgba(110,80,220,0.18)',
     position: 'relative', overflow: 'hidden',
   }}>

     <style>
       {`
         @keyframes float-slow {
           0%, 100% { transform: translateX(0px); opacity: 0.8; }
           50% { transform: translateX(350px); opacity: 1.2; }
         }
         @keyframes float-medium {
           0%, 100% { transform: translateX(0px); opacity: 0.7; }
           50% { transform: translateX(-250px); opacity: 1.1; }
         }
         @keyframes float-fast {
           0%, 100% { transform: translateX(0px); opacity: 0.9; }
           50% { transform: translateX(200px); opacity: 0.6; }
         }
         @keyframes float-diagonal {
           0%, 100% { transform: translate(0px, 0px); opacity: 0.75; }
           50% { transform: translate(120px, 30px); opacity: 1.0; }
         }
         @keyframes float-wave {
           0%, 100% { transform: translateX(0px); opacity: 0.65; }
           33% { transform: translateX(-160px); opacity: 0.9; }
           66% { transform: translateX(80px); opacity: 1.0; }
         }
         @keyframes float-pulse {
           0%, 100% { transform: scale(1); opacity: 0.8; }
           50% { transform: scale(1.3); opacity: 0.4; }
         }
         #glow-1 { animation: float-slow 8s ease-in-out infinite; }
         #glow-2 { animation: float-medium 12s ease-in-out infinite; }
         #glow-3 { animation: float-fast 9s ease-in-out infinite; }
         #glow-4 { animation: float-diagonal 10s ease-in-out infinite; }
         #glow-5 { animation: float-wave 14s ease-in-out infinite; }
       `}
     </style>

     <svg width="860" height="140" style={{ position: 'absolute', top: 0, left: 0 }}>
       <defs>
         <radialGradient id="g1" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(110,20,210,0.65)" />
           <stop offset="45%" stopColor="rgba(80,15,170,0.28)" />
           <stop offset="70%" stopColor="rgba(80,15,170,0)" />
         </radialGradient>
         <radialGradient id="g2" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(40,70,255,0.55)" />
           <stop offset="45%" stopColor="rgba(20,50,200,0.22)" />
           <stop offset="70%" stopColor="rgba(20,50,200,0)" />
         </radialGradient>
         <radialGradient id="g3" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(0,140,255,0.42)" />
           <stop offset="70%" stopColor="rgba(0,140,255,0)" />
         </radialGradient>
         <radialGradient id="g4" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(0,195,235,0.30)" />
           <stop offset="70%" stopColor="rgba(0,195,235,0)" />
         </radialGradient>
         <radialGradient id="g5" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(100,30,210,0.40)" />
           <stop offset="70%" stopColor="rgba(100,30,210,0)" />
         </radialGradient>
       </defs>
       <ellipse id="glow-1" cx="710" cy="150" rx="210" ry="150" fill="url(#g1)" />
       <ellipse id="glow-2" cx="550" cy="140" rx="190" ry="140" fill="url(#g2)" />
       <ellipse id="glow-3" cx="400" cy="130" rx="170" ry="130" fill="url(#g3)" />
       <ellipse id="glow-4" cx="250" cy="140" rx="150" ry="120" fill="url(#g4)" />
       <ellipse id="glow-5" cx="100" cy="150" rx="130" ry="110" fill="url(#g5)" />
     </svg>

     {stats.map(function(s, i) {
       return (
         <div key={s.label} style={{
           flexGrow: 1, display: 'flex', flexDirection: 'column',
           alignItems: 'center', justifyContent: 'center',
           padding: '16px 8px',
           borderRight: i < stats.length - 1 ? '1px solid rgba(255,255,255,0.06)' : 'none',
           gap: 5,
         }}>
           <div style={{ display:'flex', fontSize:30, fontWeight:800, color:s.color, lineHeight:1 }}>
             {s.value}
           </div>
           <div style={{ display:'flex', fontSize:11, color:'rgba(200,195,225,0.45)', fontWeight:600, letterSpacing:'1.5px' }}>
             {s.label.toUpperCase()}
           </div>
         </div>
       );
     })}
   </div>
 );
})()
```

```aura width=860 height=220
(function() {
 var categories = [
   { title: 'Languages', color: '#a78bfa', items: ['Python', 'TypeScript', 'JavaScript', 'C++', 'Java'] },
   { title: 'AI / Frameworks', color: '#60a5fa', items: ['LangGraph', 'TensorFlow', 'scikit-learn', 'React', 'Next.js', 'Node.js'] },
   { title: 'Cloud / Data', color: '#f59e0b', items: ['AWS', 'Azure', 'Databricks', 'PostgreSQL', 'Docker', 'MongoDB'] },
 ];

 return (
   <div style={{
     width: '100%', height: '100%',
     background: '#08080c',
     display: 'flex', flexDirection: 'column',
     fontFamily: 'Inter', padding: '18px 32px', gap: 14,
     borderRadius: 16, border: '1px solid rgba(110,80,220,0.18)',
     position: 'relative', overflow: 'hidden',
   }}>

     <style>
       {`
         @keyframes float-slow {
           0%, 100% { transform: translateX(0px); opacity: 0.8; }
           50% { transform: translateX(350px); opacity: 1.2; }
         }
         @keyframes float-medium {
           0%, 100% { transform: translateX(0px); opacity: 0.7; }
           50% { transform: translateX(-250px); opacity: 1.1; }
         }
         @keyframes float-fast {
           0%, 100% { transform: translateX(0px); opacity: 0.9; }
           50% { transform: translateX(200px); opacity: 0.6; }
         }
         @keyframes float-diagonal {
           0%, 100% { transform: translate(0px, 0px); opacity: 0.75; }
           50% { transform: translate(120px, 30px); opacity: 1.0; }
         }
         @keyframes float-wave {
           0%, 100% { transform: translateX(0px); opacity: 0.65; }
           33% { transform: translateX(-160px); opacity: 0.9; }
           66% { transform: translateX(80px); opacity: 1.0; }
         }
         @keyframes float-pulse {
           0%, 100% { transform: scale(1); opacity: 0.8; }
           50% { transform: scale(1.3); opacity: 0.4; }
         }
         #glow-1 { animation: float-slow 9s ease-in-out infinite; }
         #glow-2 { animation: float-medium 12s ease-in-out infinite; }
         #glow-3 { animation: float-fast 8s ease-in-out infinite; }
         #glow-4 { animation: float-diagonal 11s ease-in-out infinite reverse; }
         #glow-5 { animation: float-wave 14s ease-in-out infinite reverse; }
         #glow-6 { animation: float-pulse 6s ease-in-out infinite; }
       `}
     </style>

     <svg width="860" height="220" style={{ position: 'absolute', top: 0, left: 0 }}>
       <defs>
         <radialGradient id="g1" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(115,20,215,0.68)" />
           <stop offset="42%" stopColor="rgba(85,15,175,0.30)" />
           <stop offset="70%" stopColor="rgba(85,15,175,0)" />
         </radialGradient>
         <radialGradient id="g2" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(55,55,255,0.55)" />
           <stop offset="45%" stopColor="rgba(35,45,210,0.22)" />
           <stop offset="70%" stopColor="rgba(35,45,210,0)" />
         </radialGradient>
         <radialGradient id="g3" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(0,130,255,0.42)" />
           <stop offset="50%" stopColor="rgba(0,100,220,0.16)" />
           <stop offset="70%" stopColor="rgba(0,100,220,0)" />
         </radialGradient>
         <radialGradient id="g4" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(0,185,240,0.32)" />
           <stop offset="70%" stopColor="rgba(0,185,240,0)" />
         </radialGradient>
         <radialGradient id="g5" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(100,25,205,0.42)" />
           <stop offset="70%" stopColor="rgba(100,25,205,0)" />
         </radialGradient>
         <radialGradient id="g6" cx="50%" cy="50%" r="50%">
           <stop offset="0%" stopColor="rgba(60,80,255,0.35)" />
           <stop offset="70%" stopColor="rgba(60,80,255,0)" />
         </radialGradient>
       </defs>
       <ellipse id="glow-1" cx="170" cy="200" rx="260" ry="170" fill="url(#g1)" />
       <ellipse id="glow-2" cx="320" cy="210" rx="220" ry="140" fill="url(#g2)" />
       <ellipse id="glow-3" cx="460" cy="210" rx="190" ry="130" fill="url(#g3)" />
       <ellipse id="glow-4" cx="590" cy="220" rx="160" ry="110" fill="url(#g4)" />
       <ellipse id="glow-5" cx="750" cy="220" rx="140" ry="100" fill="url(#g5)" />
       <ellipse id="glow-6" cx="420" cy="170" rx="100" ry="80" fill="url(#g6)" />
     </svg>

     <div style={{ display:'flex', fontSize:10, fontWeight:700, color:'rgba(155,140,210,0.5)', letterSpacing:'3px' }}>
       TECH STACK
     </div>
     <div style={{ display:'flex', flexDirection:'column', gap:14 }}>
       {categories.map(function(cat) {
         return (
           <div key={cat.title} style={{ display:'flex', alignItems:'center', gap:16 }}>
             <div style={{ display:'flex', fontSize:10, fontWeight:700, color:cat.color, letterSpacing:'1px', width:110 }}>
               {cat.title.toUpperCase()}
             </div>
             <div style={{ display:'flex', flexWrap:'wrap', gap:7 }}>
               {cat.items.map(function(item) {
                 return (
                   <div key={item} style={{
                     display:'flex', padding:'4px 13px', borderRadius:6,
                     background:cat.color + '15', border:'1px solid ' + cat.color + '35',
                     color:'rgba(225,220,255,0.85)', fontSize:12, fontWeight:600,
                   }}>{item}</div>
                 );
               })}
             </div>
           </div>
         );
       })}
     </div>
   </div>
 );
})()
```

```aura width=130 height=44 link="https://www.linkedin.com/in/miradamkhan/" inline align=center
<SocialMediaButton
  icon="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAEAAAABACAYAAACqaXHeAAADCUlEQVR4nO2bO2zaUBSGf1dFCh1CqDOkyUBaS+mQSDgrQ+Is2RDZyJg1nRjYgaEbA1Mzhm4ZG7FFlWKpEksqxZWaoZVcCUWlSxAxi5EY3KEFEWyIr2M4+PFNGN9rn/P5Pi2ZMwwDQeYZdQDUhAKoA6Dm+bgTXL5WBJADEJtZNNNBA1ABUDHK6fvRkyYBXL62BEAGkJx6aLMhBqAA4ACAOHrSqgvk4J/kh0n+b9UPGCfAr5hysxLg9T4/CVNu4SzgtKIk8JCEZQCArN5BVluuBTVLmAVIAo/q4TYS8ejgvwI20GjrODq79pwIpi4gCTwuj1MPku+TiEdxeZyCJPCuBTcLmARUD7ddKTNP2BYgCbzlkx8lEY96qhUwCFi2fVGWstQEfhq0LUBW72xflKUsNQwCWmi09UfLNdq6p6ZCpi5wdHbtSpl5gkmArLawd1K3bAmNto69k7qnnj7gYCUoqy2sv/8c3KVwH1lteTbpYRwLmDb9xZQkLENparjXewAApdkZ/HYDZgFGOT3xPJev2S5fuviJ4sWPwbEk8MjtvEFmc2XiPRptHdWrW1S+/HqyjLloAesvX6CaFbFrcwmdiEdR2N9Abuc1cuc3qF7dOr43uQBxdRHyuxRiCxHmurGFCE6z/95zOpVAuhQW15wnP8xpVnS8ASMVkNlceXLyfYr7bx3V881maFfgIa4uMtfzjQAAONh6xVyHfBAcRev2oPzuDI6XohEkbT5ZJ+PA3AjQur2xU5ok8Khkth4VIa55tAto3R6kD/WxU5mstmztMp0MqHMhIHd+A6XZmVhGaXbw8avzBc84yAX0l7V2GB4b3IJcwKfvf2yXVZqa6/cnF0C9pSYX4ObW1gnkAliYRmshFxD4LkBNKIA6AGpCAdQBUBMKoA6AmlAAdQDUhAKoA6CGG/1miMvXfP0RkVFOc8PHgW8BoQDqAKixEuD+i7f5wZSblYDKDAKhwpSbaRYAAC5fU+C/74a+GeW0rY+mAEACUII/uoMGoGSVPDCmBQSJcBagDoCawAv4CyJz5Ou100U7AAAAAElFTkSuQmCC"
  text="LinkedIn"
  backgroundColor="#0a1a2b"
  width={130}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#ffffff' },
    { offset: '10%', color: '#111111' },
    { offset: '50%', color: '#eeeeee' },
    { offset: '60%', color: '#0A66C2' },
    { offset: '80%', color: '#111111' },
    { offset: '100%', color: '#555555' },
  ]}
/>
```

```aura width=138 height=44 link="https://x.com/adamscalesapps" inline align=center
<SocialMediaButton
  icon="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAMAAABEpIrGAAAAM1BMVEUAAAD////f398QEBAgICDv7+9wcHBAQECAgIC/v7/Pz8+vr6+QkJAwMDBQUFCfn59gYGBA/ZVxAAAA2ElEQVQ4jc1SSRLDIAzD7GuS/7+2yKQNENJrqwMMFiBbthB/gkSMrY/F/qik8d4bo69QJt9fd2SFOCh8An7k8aAIseMaw1KaslBSKig1kUL1NMFRxsIiWko98xBxWCx4s+CFihCJRquIqwsUJFZMvFKdYcFYmgvsEKAdHgQ4exOw3EucRfKXL2BoehSpBRo29EkkkbXN0LUIdzA1Q7clj3fvrt1FNoq8O9rhapj5Wv7ZoUzHWfDAXx1uUxHGjioJA07wVLCrQ4HdKdPufexD04jW/4Dl2PwELxkCBNiT/pD8AAAAAElFTkSuQmCC"
  text="X.com"
  backgroundColor="#141414"
  width={138}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#ffffff' },
    { offset: '10%', color: '#111111' },
    { offset: '50%', color: '#eeeeee' },
    { offset: '60%', color: '#ffffff' },
    { offset: '80%', color: '#111111' },
    { offset: '100%', color: '#555555' },
  ]}
/>
```

```aura width=110 height=44 link="mailto:mirkhanadam@gmail.com" inline align=center
<SocialMediaButton
  icon="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAFAklEQVRYhbVXW2xUVRRde99hpp3pdFKehYJiLZTysDyMPCSm0qAIajB+oNFEjP1AMdoETUBDAgZQJHw0GqMoIRp8kBhjNDRAgy9SBIqBQmgk0AEkLS2F0qGd6bQz52w/5nnn3rZTxPV179777LXOuefusw8hS2it8wE8KSJLAJQDKAbgjbtvA7gEoJGIDgPYz8y3s809FHGpUmqPUqpXsoRSKqSU2q21nnLHxCLiVkrtVEpFsyW2ERJRSu3QWucOd9ZTlVLn7pTYRsgZrXWJHRfZkM8VkYPMPDrTp661oO/XQ4icOonoFT90oAsQAef7YNxbDGf5XLgql8EommQ3qQ5mfoyITg8oQGs9VUTqM8lVWyuCuz5C35FfAJHBl48Irocr4FnzJozCCRYRRLSImS9aBGitPSJygpmnpw8K19Wip2Y7JNw7OHGmjlw3vOvehatiaaaIs0Q0n5l7AYATDhF5L5M89N2X6N6+adjkACC9IfQ3/GmxM/MsEdmcFBpXVSoi55jZSDjCdbXo3r7JNrmjuATOhxbBGF8EEEG1tqC/4SiizReSMTkrnoG3ej1Alm0GrXWUiMqY+SIBgFJqDzOvTgSoay24VfU8pC9sGmiML0Je9Xo45823FdZ/8hi6d26Fa3EF8taus41JE7HbMIwqEhGf1rqNmXMSzmDNGwj9fMw0YETZTPi21YC8XkuydEgoCHJ7Bo2JCwgRUSGLyIp0cun1w1W2C64HO5LBPHIU8rfsHJIcQFbkAMDMbgDLWWK1PTWD9n2AoeFe2gLPyssgp8DzylqwryCrxMOBiCxxIHawpIydvyWfnWVdcBTlwVm57K6Tx1HuQOxUSwkINpkijCkLAIdjwAyV24JZs21c6ULFdFOuYkbqSI0h0mF6pVzbEn5HaO2yVFEf2wX+X+iPWss4I9ZMpDBijOlVQhdwt+BxWYpSwIFYJzMqYaG8GZDO9mREW1cTxuooRrD9Pjj8jv1vd6lDo+pzcwkf57MI8DOAxnQLFTyafD7QNxHPtRaj9vLvtiSD4USzstimjjcyTY0c7+FSAsatQgQO7Oh5AJu75yIMA5+c/QY3w11Zk/eEBd8fj5hs94xmFGasABEdZgD7tdbJtaLcyfjMswE/hCcnAzvDAVT/sQ2B/u4hySMK2PJjHzqD5g33RLn5E8ZLcS3Hu9dv052rZq2B25FjGvD3LT9ePPg2jrT+NSD5ha4reHX/PjT4+032kR7CU3Mse+hrIupJHMdTRKSJObXTDlw5go3HamyJJucXYWHhHEzKKwQR4XrvTZy63oTGG+chEBjhErjbXwdFY+V787M5WFya+v5a60j8OG5OfhSl1A5mfiudaO/5n1Bz+qsBZzwYSHmR2/4aXp5XjtWPOE0+rfUHhmFsANJaMhFxa62PM/PM9OBD/9Rja8OnCEWH1xUZZKCq7AVUzXo6k7yRmRcQUdgkIO4sEZGjzGyqRm2hG/i4cS/qrtZDD9WUApg3dgaqZ7+EaQWmYwZa63ZmXkRE/oTNUhlEZLbW+lCmCAC4FuxA3dV6NLSfRXPgKm71BSAC+Fxe3OudgNljpqFy4kKUFtxnEaW1bieix5m50eK0CS5RSp25ixeT0yJSPCRxhohcpdSHSqnIfyDuV0q9LyI5QzMOvhpfKKWCwyAOKqV2aa3vHyq/tWceWIgXwHIxX899cXcAgB/x6zkR1RJRTzZ5/wXdyH6XrEznkwAAAABJRU5ErkJggg=="
  text="Email"
  backgroundColor="#2b0a0a"
  width={110}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#ffffff' },
    { offset: '10%', color: '#111111' },
    { offset: '50%', color: '#eeeeee' },
    { offset: '60%', color: '#EA4335' },
    { offset: '80%', color: '#111111' },
    { offset: '100%', color: '#555555' },
  ]}
/>
```

