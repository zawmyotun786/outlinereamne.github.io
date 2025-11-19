import React, { useState } from 'react';
import { Copy, Check, Shield, Sparkles, Zap, Lock } from 'lucide-react';

export default function OutlineURLRenamer() {
  const [originalUrl, setOriginalUrl] = useState('');
  const [newName, setNewName] = useState('');
  const [modifiedUrl, setModifiedUrl] = useState('');
  const [copied, setCopied] = useState(false);
  const [error, setError] = useState('');
  const [isAnimating, setIsAnimating] = useState(false);

  const handleUrlChange = (e) => {
    const url = e.target.value;
    setOriginalUrl(url);
    setError('');
    
    if (url.includes('#')) {
      const currentName = decodeURIComponent(url.split('#')[1]);
      setNewName(currentName);
    } else {
      setNewName('');
    }
    
    setModifiedUrl('');
  };

  const handleRename = () => {
    if (!originalUrl) {
      setError('Outline URL ထည့်ပါ');
      return;
    }

    if (!newName.trim()) {
      setError('အသစ်ထားမည့် နာမည်ထည့်ပါ');
      return;
    }

    try {
      if (!originalUrl.startsWith('ss://')) {
        setError('မှန်ကန်သော Outline URL မဟုတ်ပါ (ss:// နဲ့ စရပါမည်)');
        return;
      }

      setIsAnimating(true);
      setTimeout(() => {
        let baseUrl = originalUrl.split('#')[0];
        const encodedName = encodeURIComponent(newName.trim());
        const newUrl = `${baseUrl}#${encodedName}`;
        
        setModifiedUrl(newUrl);
        setError('');
        setIsAnimating(false);
      }, 800);
    } catch (err) {
      setError('URL ပြောင်းလဲရာတွင် အမှားအယွင်းရှိနေပါသည်');
      setIsAnimating(false);
    }
  };

  const handleCopy = async () => {
    if (modifiedUrl) {
      try {
        await navigator.clipboard.writeText(modifiedUrl);
        setCopied(true);
        setTimeout(() => setCopied(false), 2000);
      } catch (err) {
        alert('Copy လုပ်၍မရပါ');
      }
    }
  };

  return (
    <div className="min-h-screen bg-gradient-to-br from-purple-900 via-blue-900 to-indigo-900 p-4 sm:p-8 relative overflow-hidden">
      {/* Animated Background Elements */}
      <div className="absolute inset-0 overflow-hidden pointer-events-none">
        <div className="absolute top-1/4 left-1/4 w-96 h-96 bg-purple-500 rounded-full mix-blend-multiply filter blur-3xl opacity-20 animate-blob"></div>
        <div className="absolute top-1/3 right-1/4 w-96 h-96 bg-blue-500 rounded-full mix-blend-multiply filter blur-3xl opacity-20 animate-blob animation-delay-2000"></div>
        <div className="absolute bottom-1/4 left-1/2 w-96 h-96 bg-indigo-500 rounded-full mix-blend-multiply filter blur-3xl opacity-20 animate-blob animation-delay-4000"></div>
      </div>

      <style>{`
        @keyframes blob {
          0%, 100% { transform: translate(0, 0) scale(1); }
          33% { transform: translate(30px, -50px) scale(1.1); }
          66% { transform: translate(-20px, 20px) scale(0.9); }
        }
        .animate-blob {
          animation: blob 7s infinite;
        }
        .animation-delay-2000 {
          animation-delay: 2s;
        }
        .animation-delay-4000 {
          animation-delay: 4s;
        }
        @keyframes glow {
          0%, 100% { box-shadow: 0 0 20px rgba(139, 92, 246, 0.5), 0 0 40px rgba(59, 130, 246, 0.3); }
          50% { box-shadow: 0 0 30px rgba(139, 92, 246, 0.8), 0 0 60px rgba(59, 130, 246, 0.5); }
        }
        .glow-effect {
          animation: glow 3s ease-in-out infinite;
        }
        @keyframes shimmer {
          0% { background-position: -1000px 0; }
          100% { background-position: 1000px 0; }
        }
        .shimmer {
          background: linear-gradient(90deg, transparent, rgba(255,255,255,0.1), transparent);
          background-size: 1000px 100%;
          animation: shimmer 3s infinite;
        }
        @keyframes float {
          0%, 100% { transform: translateY(0px); }
          50% { transform: translateY(-10px); }
        }
        .float-animation {
          animation: float 3s ease-in-out infinite;
        }
      `}</style>

      <div className="max-w-4xl mx-auto relative z-10">
        {/* Glowing Header */}
        <div className="text-center mb-12 float-animation">
          <div className="inline-flex items-center justify-center mb-6">
            <div className="relative">
              <Shield className="w-20 h-20 text-purple-300 glow-effect" />
              <Sparkles className="w-8 h-8 text-yellow-300 absolute -top-2 -right-2 animate-pulse" />
            </div>
          </div>
          <h1 className="text-5xl sm:text-6xl font-black text-transparent bg-clip-text bg-gradient-to-r from-purple-400 via-pink-400 to-blue-400 mb-4 tracking-tight">
            Outline VPN
          </h1>
          <h2 className="text-3xl sm:text-4xl font-bold text-white mb-3">
            URL Renamer Pro
          </h2>
          <p className="text-purple-200 text-lg flex items-center justify-center gap-2">
            <Lock className="w-5 h-5" />
            လုံခြုံပြီး လွယ်ကူသော URL ပြောင်းလဲခြင်း
          </p>
        </div>

        {/* Main Card */}
        <div className="bg-white/10 backdrop-blur-xl rounded-3xl shadow-2xl p-8 sm:p-10 border border-white/20 shimmer">
          {/* Original URL Input */}
          <div className="mb-8">
            <label className="flex items-center gap-2 text-sm font-bold text-purple-200 mb-3 uppercase tracking-wide">
              <Zap className="w-4 h-4" />
              Outline Client URL
            </label>
            <div className="relative group">
              <textarea
                value={originalUrl}
                onChange={handleUrlChange}
                placeholder="ss://... (Outline VPN URL ထည့်ပါ)"
                className="w-full px-5 py-4 bg-white/5 border-2 border-purple-300/30 rounded-2xl focus:border-purple-400 focus:bg-white/10 focus:outline-none font-mono text-sm text-white placeholder-purple-300/50 resize-none transition-all duration-300 group-hover:border-purple-400/50"
                rows="3"
              />
              <div className="absolute inset-0 -z-10 bg-gradient-to-r from-purple-600/20 to-blue-600/20 rounded-2xl blur opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
            </div>
          </div>

          {/* New Name Input */}
          <div className="mb-8">
            <label className="flex items-center gap-2 text-sm font-bold text-purple-200 mb-3 uppercase tracking-wide">
              <Sparkles className="w-4 h-4" />
              အသစ်ထားမည့် နာမည်
            </label>
            <div className="relative group">
              <input
                type="text"
                value={newName}
                onChange={(e) => setNewName(e.target.value)}
                placeholder="ဥပမာ: My Premium VPN Server 🚀"
                className="w-full px-5 py-4 bg-white/5 border-2 border-purple-300/30 rounded-2xl focus:border-purple-400 focus:bg-white/10 focus:outline-none text-white placeholder-purple-300/50 transition-all duration-300 group-hover:border-purple-400/50"
              />
              <div className="absolute inset-0 -z-10 bg-gradient-to-r from-blue-600/20 to-purple-600/20 rounded-2xl blur opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
            </div>
          </div>

          {/* Error Message */}
          {error && (
            <div className="mb-8 p-4 bg-red-500/20 border-l-4 border-red-400 text-red-200 rounded-xl backdrop-blur-sm animate-pulse">
              <div className="flex items-center gap-2">
                <span className="text-2xl">⚠️</span>
                <span className="font-semibold">{error}</span>
              </div>
            </div>
          )}

          {/* Rename Button */}
          <button
            onClick={handleRename}
            disabled={isAnimating}
            className={`w-full bg-gradient-to-r from-purple-600 via-pink-600 to-blue-600 hover:from-purple-500 hover:via-pink-500 hover:to-blue-500 text-white font-bold py-5 px-8 rounded-2xl transition-all duration-300 transform hover:scale-105 hover:shadow-2xl mb-8 relative overflow-hidden group ${isAnimating ? 'animate-pulse' : ''}`}
          >
            <span className="relative z-10 flex items-center justify-center gap-3 text-lg">
              {isAnimating ? (
                <>
                  <div className="w-6 h-6 border-3 border-white border-t-transparent rounded-full animate-spin"></div>
                  ပြောင်းလဲနေသည်...
                </>
              ) : (
                <>
                  <Zap className="w-6 h-6" />
                  နာမည်ပြောင်းမည်
                </>
              )}
            </span>
            <div className="absolute inset-0 bg-gradient-to-r from-transparent via-white/20 to-transparent transform -skew-x-12 translate-x-full group-hover:translate-x-[-200%] transition-transform duration-1000"></div>
          </button>

          {/* Modified URL Output */}
          {modifiedUrl && (
            <div className="mb-8 animate-in fade-in slide-in-from-bottom-4 duration-500">
              <label className="flex items-center gap-2 text-sm font-bold text-green-300 mb-3 uppercase tracking-wide">
                <Check className="w-4 h-4" />
                ပြောင်းလဲပြီးသော URL
              </label>
              <div className="relative group">
                <textarea
                  value={modifiedUrl}
                  readOnly
                  className="w-full px-5 py-4 bg-green-500/10 border-2 border-green-400/50 rounded-2xl font-mono text-sm text-green-100 resize-none"
                  rows="3"
                />
                <button
                  onClick={handleCopy}
                  className="absolute top-3 right-3 bg-gradient-to-r from-green-500 to-emerald-500 hover:from-green-400 hover:to-emerald-400 text-white p-3 rounded-xl transition-all duration-300 transform hover:scale-110 shadow-lg hover:shadow-green-500/50"
                  title="Copy"
                >
                  {copied ? <Check size={22} /> : <Copy size={22} />}
                </button>
              </div>
              {copied && (
                <div className="mt-3 flex items-center gap-2 text-green-300 font-semibold animate-bounce">
                  <Check className="w-5 h-5" />
                  URL ကို clipboard သို့ copy ပြုလုပ်ပြီးပါပြီ! 🎉
                </div>
              )}
            </div>
          )}

          {/* Instructions */}
          <div className="mt-8 p-6 bg-gradient-to-br from-purple-500/10 to-blue-500/10 rounded-2xl border border-purple-300/20 backdrop-blur-sm">
            <h3 className="font-bold text-purple-200 mb-4 flex items-center gap-2 text-lg">
              <Sparkles className="w-5 h-5" />
              အသုံးပြုနည်း
            </h3>
            <div className="space-y-3 text-purple-100">
              <div className="flex items-start gap-3">
                <div className="w-8 h-8 rounded-full bg-purple-500 flex items-center justify-center flex-shrink-0 font-bold">1</div>
                <p>Outline VPN client URL ကို အပေါ်က box မှာ paste လုပ်ပါ</p>
              </div>
              <div className="flex items-start gap-3">
                <div className="w-8 h-8 rounded-full bg-pink-500 flex items-center justify-center flex-shrink-0 font-bold">2</div>
                <p>သင်နှစ်သက်သော နာမည်အသစ်ကို ထည့်သွင်းပါ</p>
              </div>
              <div className="flex items-start gap-3">
                <div className="w-8 h-8 rounded-full bg-blue-500 flex items-center justify-center flex-shrink-0 font-bold">3</div>
                <p>"နာမည်ပြောင်းမည်" ခလုတ်ကို နှိပ်ပါ</p>
              </div>
              <div className="flex items-start gap-3">
                <div className="w-8 h-8 rounded-full bg-green-500 flex items-center justify-center flex-shrink-0 font-bold">4</div>
                <p>ပြောင်းလဲပြီးသော URL ကို copy icon နှိပ်ပြီး အသုံးပြုပါ</p>
              </div>
            </div>
          </div>
        </div>

        {/* Footer */}
        <div className="text-center mt-8 text-purple-300/70 text-sm">
          <p className="flex items-center justify-center gap-2">
            <Shield className="w-4 h-4" />
            Safe • Secure • Private
          </p>
        </div>
      </div>
    </div>
  );
}
