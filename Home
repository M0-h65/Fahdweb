import React, { useState, useEffect } from 'react';
import { Menu, X, Moon, Sun, ChevronDown, Play, Camera, Zap, TrendingUp, Film, Edit3, Smartphone, Award, Users, Target, ArrowRight, Check, ChevronRight, Mail, Phone, MapPin, Clock } from 'lucide-react';

/**
 * Design Philosophy: Premium Dark Mode with Modern Arabic Support
 * - Color Scheme: Deep Navy (#0A0B14) with Coral Accent (#FF6B4A)
 * - Typography: Bold headings with light gray body text
 * - Layout: RTL-first with glassmorphism effects
 * - Animations: Smooth scroll reveals and hover effects
 */

export default function Home() {
  const [currentPage, setCurrentPage] = useState('home');
  const [mobileMenuOpen, setMobileMenuOpen] = useState(false);
  const [darkMode, setDarkMode] = useState(true);
  const [scrolled, setScrolled] = useState(false);

  useEffect(() => {
    const handleScroll = () => {
      setScrolled(window.scrollY > 50);
    };
    window.addEventListener('scroll', handleScroll);
    return () => window.removeEventListener('scroll', handleScroll);
  }, []);

  // ==================== HOME PAGE ====================
  const HomePage = () => (
    <div className="min-h-screen" dir="rtl">
      {/* Hero Section */}
      <section className="relative min-h-screen bg-gradient-to-b from-[#0A0B14] via-[#0F1220] to-[#0A0B14] flex items-center justify-center overflow-hidden pt-20">
        {/* Animated background elements */}
        <div className="absolute inset-0 overflow-hidden">
          <div className="absolute top-20 right-10 w-72 h-72 bg-[#FF6B4A] rounded-full mix-blend-multiply filter blur-3xl opacity-10 animate-pulse"></div>
          <div className="absolute bottom-20 left-10 w-72 h-72 bg-purple-600 rounded-full mix-blend-multiply filter blur-3xl opacity-10 animate-pulse" style={{ animationDelay: '2s' }}></div>
        </div>

        <div className="relative z-10 container mx-auto px-4 text-center">
          <h1 className="text-5xl md:text-7xl font-black text-white mb-6 leading-tight">
            الهدف الأمثل <span className="text-[#FF6B4A]">للتسويق</span>
          </h1>
          <p className="text-xl md:text-2xl text-[#A0A0A0] mb-12 max-w-2xl mx-auto">
            نحن نحول أفكارك إلى محتوى بصري احترافي يترك انطباعاً دائماً
          </p>

          {/* Main CTA Buttons */}
          <div className="flex flex-col md:flex-row gap-6 justify-center items-center mb-16">
            <button
              onClick={() => setCurrentPage('photography')}
              className="px-8 py-4 bg-[#FF6B4A] text-white rounded-lg font-bold text-lg hover:bg-[#E55A39] transition-all duration-300 transform hover:scale-105 flex items-center gap-3 group"
            >
              <Camera size={24} className="group-hover:rotate-12 transition-transform" />
              التصوير الفوتوغرافي
            </button>
            <button
              onClick={() => setCurrentPage('video')}
              className="px-8 py-4 border-2 border-[#FF6B4A] text-[#FF6B4A] rounded-lg font-bold text-lg hover:bg-[#FF6B4A] hover:text-white transition-all duration-300 transform hover:scale-105 flex items-center gap-3 group"
            >
              <Film size={24} className="group-hover:rotate-12 transition-transform" />
              المونتاج والفيديو
            </button>
          </div>

          {/* About Section */}
          <div className="grid md:grid-cols-3 gap-8 mt-20">
            <div className="bg-white/5 backdrop-blur-md border border-white/10 rounded-2xl p-8 hover:border-[#FF6B4A]/50 transition-all duration-300 transform hover:translate-y-[-8px]">
              <div className="text-4xl mb-4">🎯</div>
              <h3 className="text-white font-bold text-xl mb-3">من نحن</h3>
              <p className="text-[#A0A0A0]">فريق متخصص في إنتاج محتوى بصري احترافي يجمع بين الإبداع والتقنية الحديثة</p>
            </div>
            <div className="bg-white/5 backdrop-blur-md border border-white/10 rounded-2xl p-8 hover:border-[#FF6B4A]/50 transition-all duration-300 transform hover:translate-y-[-8px]">
              <div className="text-4xl mb-4">⚡</div>
              <h3 className="text-white font-bold text-xl mb-3">خبرتنا</h3>
              <p className="text-[#A0A0A0]">أكثر من 500 مشروع ناجح مع علامات تجارية رائدة في السعودية والخليج</p>
            </div>
            <div className="bg-white/5 backdrop-blur-md border border-white/10 rounded-2xl p-8 hover:border-[#FF6B4A]/50 transition-all duration-300 transform hover:translate-y-[-8px]">
              <div className="text-4xl mb-4">🚀</div>
              <h3 className="text-white font-bold text-xl mb-3">رؤيتنا</h3>
              <p className="text-[#A0A0A0]">تقديم خدمات تسويقية بصرية تحقق نتائج قابلة للقياس والتتبع</p>
            </div>
          </div>
        </div>
      </section>

      {/* Services Preview */}
      <section className="bg-[#0F1220] py-20 px-4">
        <div className="container mx-auto">
          <h2 className="text-4xl font-black text-white text-center mb-16">خدماتنا الرئيسية</h2>
          <div className="grid md:grid-cols-2 gap-12">
            {/* Photography Card */}
            <div
              onClick={() => setCurrentPage('photography')}
              className="bg-gradient-to-br from-[#1A1D2E] to-[#0F1220] border border-white/10 rounded-2xl p-8 cursor-pointer hover:border-[#FF6B4A]/50 transition-all duration-300 group hover:shadow-2xl hover:shadow-[#FF6B4A]/20"
            >
              <div className="text-6xl mb-4 group-hover:scale-110 transition-transform">📸</div>
              <h3 className="text-2xl font-bold text-white mb-3">التصوير الفوتوغرافي</h3>
              <p className="text-[#A0A0A0] mb-6">
                جلسات تصوير احترافية بأحدث المعدات والتقنيات لتصوير منتجاتك وفريقك بأفضل صورة
              </p>
              <div className="flex items-center text-[#FF6B4A] font-bold group-hover:gap-3 gap-1 transition-all">
                اكتشف المزيد
                <ArrowRight size={20} className="group-hover:translate-x-2 transition-transform" />
              </div>
            </div>

            {/* Video Card */}
            <div
              onClick={() => setCurrentPage('video')}
              className="bg-gradient-to-br from-[#1A1D2E] to-[#0F1220] border border-white/10 rounded-2xl p-8 cursor-pointer hover:border-[#FF6B4A]/50 transition-all duration-300 group hover:shadow-2xl hover:shadow-[#FF6B4A]/20"
            >
              <div className="text-6xl mb-4 group-hover:scale-110 transition-transform">🎬</div>
              <h3 className="text-2xl font-bold text-white mb-3">المونتاج والفيديو</h3>
              <p className="text-[#A0A0A0] mb-6">
                إنتاج فيديوهات احترافية وعالية الجودة مع مونتاج متقن وتأثيرات بصرية مذهلة
              </p>
              <div className="flex items-center text-[#FF6B4A] font-bold group-hover:gap-3 gap-1 transition-all">
                اكتشف المزيد
                <ArrowRight size={20} className="group-hover:translate-x-2 transition-transform" />
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* Stats Section */}
      <section className="bg-[#0A0B14] py-20 px-4">
        <div className="container mx-auto">
          <div className="grid md:grid-cols-4 gap-8 text-center">
            <div>
              <div className="text-5xl font-black text-[#FF6B4A] mb-2">500+</div>
              <p className="text-[#A0A0A0]">مشروع منجز</p>
            </div>
            <div>
              <div className="text-5xl font-black text-[#FF6B4A] mb-2">150+</div>
              <p className="text-[#A0A0A0]">عميل سعيد</p>
            </div>
            <div>
              <div className="text-5xl font-black text-[#FF6B4A] mb-2">8+</div>
              <p className="text-[#A0A0A0]">سنوات خبرة</p>
            </div>
            <div>
              <div className="text-5xl font-black text-[#FF6B4A] mb-2">24/7</div>
              <p className="text-[#A0A0A0]">دعم فني</p>
            </div>
          </div>
        </div>
      </section>
    </div>
  );

  // ==================== PHOTOGRAPHY PAGE ====================
  const PhotographyPage = () => (
    <div className="min-h-screen" dir="rtl">
      {/* Hero Section */}
      <section className="relative min-h-screen bg-gradient-to-b from-[#0A0B14] via-[#0F1220] to-[#0A0B14] flex items-center justify-center overflow-hidden pt-20">
        <div className="absolute inset-0 overflow-hidden">
          <div className="absolute top-20 right-10 w-72 h-72 bg-[#FF6B4A] rounded-full mix-blend-multiply filter blur-3xl opacity-10 animate-pulse"></div>
        </div>

        <div className="relative z-10 container mx-auto px-4">
          <div className="text-center mb-12">
            <div className="inline-block bg-[#FF6B4A]/20 border border-[#FF6B4A] text-[#FF6B4A] px-4 py-2 rounded-full font-bold mb-6">
              📸 التصوير الاحترافي
            </div>
            <h1 className="text-5xl md:text-6xl font-black text-white mb-6">
              التصوير الفوتوغرافي <span className="text-[#FF6B4A]">الاحترافي</span>
            </h1>
            <p className="text-xl text-[#A0A0A0] max-w-3xl mx-auto mb-12">
              نحول لحظاتك إلى ذكريات خالدة بجودة عالية وإبداع بصري لا مثيل له
            </p>
          </div>

          {/* Quick Features */}
          <div className="grid md:grid-cols-2 gap-4 mb-12">
            <div className="bg-[#1A1D2E]/50 backdrop-blur border border-white/10 rounded-xl p-4 flex items-center gap-4">
              <Zap className="text-[#FF6B4A]" size={24} />
              <div className="text-right">
                <p className="text-white font-bold">معدات احترافية</p>
                <p className="text-[#A0A0A0] text-sm">أحدث كاميرات وعدسات</p>
              </div>
            </div>
            <div className="bg-[#1A1D2E]/50 backdrop-blur border border-white/10 rounded-xl p-4 flex items-center gap-4">
              <Award className="text-[#FF6B4A]" size={24} />
              <div className="text-right">
                <p className="text-white font-bold">فريق محترف</p>
                <p className="text-[#A0A0A0] text-sm">خبرة تزيد عن 8 سنوات</p>
              </div>
            </div>
            <div className="bg-[#1A1D2E]/50 backdrop-blur border border-white/10 rounded-xl p-4 flex items-center gap-4">
              <TrendingUp className="text-[#FF6B4A]" size={24} />
              <div className="text-right">
                <p className="text-white font-bold">نتائج مثبتة</p>
                <p className="text-[#A0A0A0] text-sm">زيادة المبيعات والتفاعل</p>
              </div>
            </div>
            <div className="bg-[#1A1D2E]/50 backdrop-blur border border-white/10 rounded-xl p-4 flex items-center gap-4">
              <Users className="text-[#FF6B4A]" size={24} />
              <div className="text-right">
                <p className="text-white font-bold">فريق ديناميكي</p>
                <p className="text-[#A0A0A0] text-sm">متعاون وملتزم</p>
              </div>
            </div>
          </div>

          {/* CTA Buttons */}
          <div className="flex flex-col md:flex-row gap-6 justify-center">
            <button className="px-8 py-4 bg-[#FF6B4A] text-white rounded-lg font-bold text-lg hover:bg-[#E55A39] transition-all duration-300 transform hover:scale-105">
              احجز جلسة تصوير الآن
            </button>
            <button className="px-8 py-4 border-2 border-[#FF6B4A] text-[#FF6B4A] rounded-lg font-bold text-lg hover:bg-[#FF6B4A] hover:text-white transition-all duration-300 flex items-center gap-2 justify-center">
              <Play size={20} />
              شاهد معرض أعمالنا
            </button>
          </div>
        </div>
      </section>

      {/* Why Professional Photography */}
      <section className="bg-[#0F1220] py-20 px-4">
        <div className="container mx-auto">
          <h2 className="text-4xl font-black text-white text-center mb-16">
            لماذا التصوير <span className="text-[#FF6B4A]">الاحترافي</span>؟
          </h2>
          <div className="grid md:grid-cols-3 gap-8">
            {[
              { icon: '📈', title: 'زيادة المبيعات', desc: 'صور عالية الجودة تزيد من ثقة العملاء وتحفزهم على الشراء' },
              { icon: '✨', title: 'تعزيز العلامة التجارية', desc: 'محتوى بصري احترافي يعكس احترافية علامتك التجارية' },
              { icon: '🎯', title: 'تحسين التفاعل', desc: 'صور جذابة تزيد من تفاعل المتابعين على وسائل التواصل' },
            ].map((item, idx) => (
              <div key={idx} className="bg-white/5 backdrop-blur-md border border-white/10 rounded-2xl p-8 hover:border-[#FF6B4A]/50 transition-all duration-300 transform hover:translate-y-[-8px]">
                <div className="text-5xl mb-4">{item.icon}</div>
                <h3 className="text-white font-bold text-xl mb-3">{item.title}</h3>
                <p className="text-[#A0A0A0]">{item.desc}</p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Services Offered */}
      <section className="bg-[#0A0B14] py-20 px-4">
        <div className="container mx-auto">
          <h2 className="text-4xl font-black text-white text-center mb-16">أنواع التصوير التي نقدمها</h2>
          <div className="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
            {[
              { icon: '🏢', title: 'تصوير المنتجات', desc: 'صور احترافية للمنتجات' },
              { icon: '👥', title: 'تصوير الفريق', desc: 'صور فريق العمل والموظفين' },
              { icon: '🎪', title: 'تصوير الفعاليات', desc: 'توثيق الفعاليات والحفلات' },
              { icon: '🏠', title: 'تصوير العقارات', desc: 'صور احترافية للعقارات' },
            ].map((item, idx) => (
              <div key={idx} className="bg-[#1A1D2E] border border-white/10 rounded-xl p-6 hover:border-[#FF6B4A]/50 transition-all duration-300 text-center">
                <div className="text-4xl mb-3">{item.icon}</div>
                <h3 className="text-white font-bold mb-2">{item.title}</h3>
                <p className="text-[#A0A0A0] text-sm">{item.desc}</p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Process Section */}
      <section className="bg-[#0F1220] py-20 px-4">
        <div className="container mx-auto">
          <h2 className="text-4xl font-black text-white text-center mb-16">رحلة التصوير معنا</h2>
          <div className="max-w-2xl mx-auto">
            {[
              { num: '01', title: 'الاستشارة', desc: 'نستمع لأفكارك ونفهم احتياجاتك بدقة' },
              { num: '02', title: 'التخطيط', desc: 'نضع خطة تفصيلية للجلسة وأهدافها' },
              { num: '03', title: 'التصوير', desc: 'تنفيذ الجلسة بمحترفية وإبداع عالي' },
              { num: '04', title: 'المعالجة', desc: 'تحرير واستخراج أفضل الصور' },
              { num: '05', title: 'التسليم', desc: 'تسليم الصور بجودة عالية جاهزة للاستخدام' },
            ].map((step, idx) => (
              <div key={idx} className="flex gap-6 mb-8 relative">
                <div className="flex flex-col items-center">
                  <div className="w-16 h-16 bg-[#FF6B4A] rounded-full flex items-center justify-center text-white font-black text-xl mb-4 z-10">
                    {step.num}
                  </div>
                  {idx < 4 && <div className="w-1 h-16 bg-[#FF6B4A]/30"></div>}
                </div>
                <div className="pb-8">
                  <h3 className="text-white font-bold text-xl mb-2">{step.title}</h3>
                  <p className="text-[#A0A0A0]">{step.desc}</p>
                </div>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Pricing */}
      <section className="bg-[#0A0B14] py-20 px-4">
        <div className="container mx-auto">
          <h2 className="text-4xl font-black text-white text-center mb-16">باقات التصوير</h2>
          <div className="grid md:grid-cols-3 gap-8">
            {[
              { name: 'باقة أساسية', price: '1,500', features: ['4 ساعات تصوير', '100+ صورة', 'معالجة أساسية', 'تسليم رقمي'] },
              { name: 'باقة احترافية', price: '2,500', features: ['8 ساعات تصوير', '250+ صورة', 'معالجة متقدمة', 'ألبوم رقمي', 'نسخة مطبوعة'], featured: true },
              { name: 'باقة فاخرة', price: '4,000', features: ['يوم كامل', '500+ صورة', 'معالجة احترافية', 'ألبوم فاخر', 'فيديو قصير', 'جلسة متابعة'] },
            ].map((pkg, idx) => (
              <div key={idx} className={`rounded-2xl p-8 transition-all duration-300 ${pkg.featured ? 'bg-gradient-to-br from-[#FF6B4A] to-[#E55A39] text-white scale-105 shadow-2xl shadow-[#FF6B4A]/50' : 'bg-[#1A1D2E] border border-white/10 text-white hover:border-[#FF6B4A]/50'}`}>
                {pkg.featured && <div className="text-center mb-4 font-bold text-sm">الأكثر طلباً</div>}
                <h3 className="text-2xl font-bold mb-2">{pkg.name}</h3>
                <div className="text-4xl font-black mb-6">{pkg.price} <span className="text-lg">ريال</span></div>
                <ul className="space-y-3 mb-8">
                  {pkg.features.map((feature, fidx) => (
                    <li key={fidx} className="flex items-center gap-2">
                      <Check size={20} />
                      {feature}
                    </li>
                  ))}
                </ul>
                <button className={`w-full py-3 rounded-lg font-bold transition-all duration-300 ${pkg.featured ? 'bg-white text-[#FF6B4A] hover:bg-gray-100' : 'border-2 border-[#FF6B4A] text-[#FF6B4A] hover:bg-[#FF6B4A] hover:text-white'}`}>
                  احجز الآن
                </button>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* CTA Section */}
      <section className="bg-gradient-to-r from-[#FF6B4A] to-[#E55A39] py-16 px-4">
        <div className="container mx-auto text-center text-white">
          <h2 className="text-4xl font-black mb-6">جاهز لجلسة تصوير احترافية؟</h2>
          <p className="text-xl mb-8 opacity-90">تواصل معنا اليوم واحصل على استشارة مجانية</p>
          <button className="px-8 py-4 bg-white text-[#FF6B4A] rounded-lg font-bold text-lg hover:bg-gray-100 transition-all duration-300 transform hover:scale-105">
            احجز الآن
          </button>
        </div>
      </section>
    </div>
  );

  // ==================== VIDEO PAGE ====================
  const VideoPage = () => (
    <div className="min-h-screen" dir="rtl">
      {/* Hero Section */}
      <section className="relative min-h-screen bg-gradient-to-b from-[#050814] via-[#0a0f1a] to-[#050814] flex items-center justify-center overflow-hidden pt-20">
        <div className="absolute inset-0 overflow-hidden">
          <div className="absolute top-20 right-10 w-72 h-72 bg-pink-600 rounded-full mix-blend-multiply filter blur-3xl opacity-10 animate-pulse"></div>
          <div className="absolute bottom-20 left-10 w-72 h-72 bg-blue-600 rounded-full mix-blend-multiply filter blur-3xl opacity-10 animate-pulse" style={{ animationDelay: '2s' }}></div>
        </div>

        <div className="relative z-10 container mx-auto px-4">
          <div className="text-center mb-12">
            <div className="inline-block bg-red-900/30 border border-red-600 text-red-400 px-4 py-2 rounded-full font-bold mb-6">
              🎥 إنتاج فيديو احترافي
            </div>
            <h1 className="text-5xl md:text-6xl font-black text-white mb-6">
              إنتاج فيديو ومونتاج <span className="bg-gradient-to-r from-pink-500 to-red-500 bg-clip-text text-transparent">احترافي</span>
            </h1>
            <p className="text-xl text-[#A0A0A0] max-w-3xl mx-auto mb-12">
              يضع علامتك في مستوى أعلى من المنافسة
            </p>
          </div>

          {/* Quick Features */}
          <div className="grid md:grid-cols-2 gap-4 mb-12">
            <div className="bg-[#0a0f1a]/50 backdrop-blur border border-white/10 rounded-xl p-4 flex items-center gap-4">
              <Zap className="text-pink-500" size={24} />
              <div className="text-right">
                <p className="text-white font-bold">4K وأعلى</p>
                <p className="text-[#A0A0A0] text-sm">جودة سينمائية احترافية</p>
              </div>
            </div>
            <div className="bg-[#0a0f1a]/50 backdrop-blur border border-white/10 rounded-xl p-4 flex items-center gap-4">
              <Award className="text-pink-500" size={24} />
              <div className="text-right">
                <p className="text-white font-bold">فريق محترف</p>
                <p className="text-[#A0A0A0] text-sm">خبرة تزيد عن 8 سنوات</p>
              </div>
            </div>
            <div className="bg-[#0a0f1a]/50 backdrop-blur border border-white/10 rounded-xl p-4 flex items-center gap-4">
              <TrendingUp className="text-pink-500" size={24} />
              <div className="text-right">
                <p className="text-white font-bold">نتائج مثبتة</p>
                <p className="text-[#A0A0A0] text-sm">زيادة المبيعات والتفاعل</p>
              </div>
            </div>
            <div className="bg-[#0a0f1a]/50 backdrop-blur border border-white/10 rounded-xl p-4 flex items-center gap-4">
              <Users className="text-pink-500" size={24} />
              <div className="text-right">
                <p className="text-white font-bold">فريق ديناميكي</p>
                <p className="text-[#A0A0A0] text-sm">متعاون وملتزم</p>
              </div>
            </div>
          </div>

          {/* CTA Buttons */}
          <div className="flex flex-col md:flex-row gap-6 justify-center">
            <button className="px-8 py-4 bg-gradient-to-r from-pink-500 to-red-500 text-white rounded-lg font-bold text-lg hover:shadow-lg hover:shadow-pink-500/50 transition-all duration-300 transform hover:scale-105">
              اطلب عرض سعر للفيديو الآن
            </button>
            <button className="px-8 py-4 border-2 border-pink-500 text-pink-400 rounded-lg font-bold text-lg hover:bg-pink-500/10 transition-all duration-300 flex items-center gap-2 justify-center">
              <Play size={20} />
              شاهد نماذج من أعمالنا
            </button>
          </div>
        </div>
      </section>

      {/* Benefits Section */}
      <section className="bg-[#0a0f1a] py-20 px-4">
        <div className="container mx-auto">
          <h2 className="text-4xl font-black text-white text-center mb-4">
            لماذا الفيديو مهم <span className="text-blue-400">لعلامتك</span>؟
          </h2>
          <p className="text-center text-[#A0A0A0] mb-16 max-w-2xl mx-auto">
            الفيديو هو أقوى أداة تسويقية في العصر الرقمي
          </p>
          <div className="grid md:grid-cols-3 gap-8">
            {[
              { icon: '📈', title: 'الفيديو يرفع التفاعل أضعافاً', desc: 'محتوى الفيديو يحصل على 1200% مرات أكثر من النصوص والصور مجتمعة' },
              { icon: '💰', title: 'زيادة المبيعات والتحويلات', desc: 'المتاجر التي تستخدم الفيديو تحقق مبيعات أعلى بـ 80% من غيرها' },
              { icon: '🎯', title: 'بناء ثقة العملاء', desc: 'الفيديو يعطي صورة احترافية وموثوقة عن علامتك التجارية' },
            ].map((item, idx) => (
              <div key={idx} className="bg-[#0f1420]/80 backdrop-blur border border-white/10 rounded-2xl p-8 hover:border-pink-500/50 transition-all duration-300 transform hover:translate-y-[-8px]">
                <div className="text-5xl mb-4">{item.icon}</div>
                <h3 className="text-white font-bold text-xl mb-3">{item.title}</h3>
                <p className="text-[#A0A0A0]">{item.desc}</p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Services Offered */}
      <section className="bg-[#050814] py-20 px-4">
        <div className="container mx-auto">
          <h2 className="text-4xl font-black text-white text-center mb-16">أنواع الفيديوهات التي ننتجها</h2>
          <div className="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
            {[
              { icon: '📱', title: 'فيديوهات ريلز', desc: 'محتوى قصير جذاب' },
              { icon: '🎬', title: 'فيديوهات ترويجية', desc: 'إعلانات احترافية' },
              { icon: '📦', title: 'فيديوهات المنتجات', desc: 'عرض المنتجات بجودة عالية' },
              { icon: '🎓', title: 'فيديوهات تعليمية', desc: 'شروحات وتوثيق' },
            ].map((item, idx) => (
              <div key={idx} className="bg-[#0f1420] border border-white/10 rounded-xl p-6 hover:border-pink-500/50 transition-all duration-300 text-center">
                <div className="text-4xl mb-3">{item.icon}</div>
                <h3 className="text-white font-bold mb-2">{item.title}</h3>
                <p className="text-[#A0A0A0] text-sm">{item.desc}</p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Process Timeline */}
      <section className="bg-[#0a0f1a] py-20 px-4">
        <div className="container mx-auto">
          <h2 className="text-4xl font-black text-white text-center mb-16">رحلة إنتاج الفيديو</h2>
          <div className="max-w-2xl mx-auto">
            {[
              { num: '01', title: 'التخطيط والسيناريو', desc: 'نضع خطة تفصيلية وسيناريو احترافي' },
              { num: '02', title: 'الإنتاج', desc: 'تصوير احترافي بأحدث المعدات' },
              { num: '03', title: 'المونتاج', desc: 'تحرير واستخراج أفضل اللقطات' },
              { num: '04', title: 'التأثيرات والرسوميات', desc: 'إضافة تأثيرات بصرية مذهلة' },
              { num: '05', title: 'المراجعة والتسليم', desc: 'مراجعة نهائية وتسليم الفيديو' },
            ].map((step, idx) => (
              <div key={idx} className="flex gap-6 mb-8 relative">
                <div className="flex flex-col items-center">
                  <div className="w-16 h-16 bg-gradient-to-r from-pink-500 to-red-500 rounded-full flex items-center justify-center text-white font-black text-xl mb-4 z-10">
                    {step.num}
                  </div>
                  {idx < 4 && <div className="w-1 h-16 bg-pink-500/30"></div>}
                </div>
                <div className="pb-8">
                  <h3 className="text-white font-bold text-xl mb-2">{step.title}</h3>
                  <p className="text-[#A0A0A0]">{step.desc}</p>
                </div>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Pricing */}
      <section className="bg-[#050814] py-20 px-4">
        <div className="container mx-auto">
          <h2 className="text-4xl font-black text-white text-center mb-16">باقات إنتاج الفيديو</h2>
          <div className="grid md:grid-cols-3 gap-8">
            {[
              { name: 'Social Clips', price: '2,000', features: ['فيديوهات قصيرة', 'مدة 15-30 ثانية', 'مونتاج احترافي', 'موسيقى وتأثيرات'] },
              { name: 'Business Promo', price: '5,000', features: ['فيديو ترويجي', 'مدة 1-2 دقيقة', 'سيناريو احترافي', 'رسوميات متقدمة', 'موسيقى مخصصة'], featured: true },
              { name: 'Elite Production', price: '10,000', features: ['فيديو سينمائي', 'مدة 3-5 دقائق', 'إنتاج كامل', 'تأثيرات احترافية', 'دعم ما بعد الإنتاج'] },
            ].map((pkg, idx) => (
              <div key={idx} className={`rounded-2xl p-8 transition-all duration-300 ${pkg.featured ? 'bg-gradient-to-br from-pink-600 to-red-600 text-white scale-105 shadow-2xl shadow-pink-500/50' : 'bg-[#0f1420] border border-white/10 text-white hover:border-pink-500/50'}`}>
                {pkg.featured && <div className="text-center mb-4 font-bold text-sm">الأكثر طلباً</div>}
                <h3 className="text-2xl font-bold mb-2">{pkg.name}</h3>
                <div className="text-4xl font-black mb-6">{pkg.price} <span className="text-lg">ريال</span></div>
                <ul className="space-y-3 mb-8">
                  {pkg.features.map((feature, fidx) => (
                    <li key={fidx} className="flex items-center gap-2">
                      <Check size={20} />
                      {feature}
                    </li>
                  ))}
                </ul>
                <button className={`w-full py-3 rounded-lg font-bold transition-all duration-300 ${pkg.featured ? 'bg-white text-pink-600 hover:bg-gray-100' : 'border-2 border-pink-500 text-pink-400 hover:bg-pink-500/10'}`}>
                  احجز الآن
                </button>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Stats */}
      <section className="bg-[#0a0f1a] py-20 px-4">
        <div className="container mx-auto">
          <h2 className="text-4xl font-black text-white text-center mb-16">نتائج ملموسة</h2>
          <div className="grid md:grid-cols-4 gap-8 text-center">
            {[
              { num: '+128%', label: 'متوسط زيادة التفاعل' },
              { num: '+198%', label: 'زيادة المبيعات' },
              { num: '+85%', label: 'تحسن معدل التحويل' },
              { num: '+250%', label: 'زيادة الوعي بالعلامة' },
            ].map((stat, idx) => (
              <div key={idx}>
                <div className="text-5xl font-black bg-gradient-to-r from-pink-500 to-red-500 bg-clip-text text-transparent mb-2">{stat.num}</div>
                <p className="text-[#A0A0A0]">{stat.label}</p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Tools & Quality */}
      <section className="bg-[#050814] py-20 px-4">
        <div className="container mx-auto">
          <h2 className="text-4xl font-black text-white text-center mb-16">الأدوات والجودة</h2>
          <div className="grid md:grid-cols-4 gap-6">
            {[
              { icon: '📹', title: '4K Cameras', desc: 'كاميرات احترافية' },
              { icon: '✂️', title: 'Adobe Premiere', desc: 'مونتاج احترافي' },
              { icon: '✨', title: 'After Effects', desc: 'تأثيرات متقدمة' },
              { icon: '🎵', title: 'Licensed Music', desc: 'موسيقى مرخصة' },
            ].map((tool, idx) => (
              <div key={idx} className="bg-[#0f1420] border border-white/10 rounded-xl p-6 hover:border-pink-500/50 transition-all duration-300 text-center">
                <div className="text-4xl mb-3">{tool.icon}</div>
                <h3 className="text-white font-bold mb-2">{tool.title}</h3>
                <p className="text-[#A0A0A0] text-sm">{tool.desc}</p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* FAQ */}
      <section className="bg-[#0a0f1a] py-20 px-4">
        <div className="container mx-auto max-w-3xl">
          <h2 className="text-4xl font-black text-white text-center mb-16">الأسئلة الشائعة</h2>
          <div className="space-y-4">
            {[
              { q: 'كم المدة المتوقعة لإنتاج الفيديو؟', a: 'عادة ما تستغرق من 2-4 أسابيع حسب حجم المشروع' },
              { q: 'هل تقدمون خدمات التعديل بعد الإنتاج؟', a: 'نعم، نقدم خدمات تعديل مجانية خلال 30 يوم' },
              { q: 'هل يمكنكم إنتاج فيديو بلغات أخرى؟', a: 'بالتأكيد، نتعامل مع عدة لغات وثقافات' },
            ].map((item, idx) => (
              <div key={idx} className="bg-[#0f1420] border border-white/10 rounded-xl p-6 hover:border-pink-500/50 transition-all duration-300">
                <div className="flex items-center justify-between cursor-pointer">
                  <h3 className="text-white font-bold">{item.q}</h3>
                  <ChevronDown size={24} className="text-pink-500" />
                </div>
                <p className="text-[#A0A0A0] mt-4">{item.a}</p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Final CTA */}
      <section className="bg-gradient-to-r from-pink-600 to-red-600 py-16 px-4">
        <div className="container mx-auto text-center text-white">
          <h2 className="text-4xl font-black mb-6">جاهز لبدء مشروعك معنا؟</h2>
          <p className="text-xl mb-8 opacity-90">تواصل معنا اليوم واحصل على استشارة مجانية</p>
          <button className="px-8 py-4 bg-white text-pink-600 rounded-lg font-bold text-lg hover:bg-gray-100 transition-all duration-300 transform hover:scale-105">
            اطلب عرض سعر الآن
          </button>
        </div>
      </section>
    </div>
  );

  // ==================== HEADER ====================
  const Header = () => (
    <header className={`fixed top-0 right-0 left-0 z-50 transition-all duration-300 ${scrolled ? 'bg-[#0A0B14]/95 backdrop-blur-md border-b border-white/10' : 'bg-transparent'}`} dir="rtl">
      <div className="container mx-auto px-4 py-4 flex items-center justify-between">
        {/* Logo */}
        <div className="flex items-center gap-3 cursor-pointer" onClick={() => setCurrentPage('home')}>
          <div className="text-3xl font-black bg-gradient-to-r from-[#FF6B4A] to-pink-500 bg-clip-text text-transparent">
            الهدف الأمثل
          </div>
        </div>

        {/* Desktop Navigation */}
        <nav className="hidden md:flex items-center gap-8">
          <button onClick={() => setCurrentPage('home')} className={`font-bold transition-colors ${currentPage === 'home' ? 'text-[#FF6B4A]' : 'text-[#A0A0A0] hover:text-white'}`}>
            الرئيسية
          </button>
          <button onClick={() => setCurrentPage('photography')} className={`font-bold transition-colors ${currentPage === 'photography' ? 'text-[#FF6B4A]' : 'text-[#A0A0A0] hover:text-white'}`}>
            التصوير
          </button>
          <button onClick={() => setCurrentPage('video')} className={`font-bold transition-colors ${currentPage === 'video' ? 'text-[#FF6B4A]' : 'text-[#A0A0A0] hover:text-white'}`}>
            الفيديو
          </button>
        </nav>

        {/* Right Actions */}
        <div className="flex items-center gap-4">
          <button onClick={() => setDarkMode(!darkMode)} className="p-2 hover:bg-white/10 rounded-lg transition-colors">
            {darkMode ? <Sun size={24} className="text-[#FF6B4A]" /> : <Moon size={24} className="text-[#FF6B4A]" />}
          </button>
          <button onClick={() => setMobileMenuOpen(!mobileMenuOpen)} className="md:hidden p-2 hover:bg-white/10 rounded-lg transition-colors">
            {mobileMenuOpen ? <X size={24} className="text-white" /> : <Menu size={24} className="text-white" />}
          </button>
        </div>
      </div>

      {/* Mobile Menu */}
      {mobileMenuOpen && (
        <div className="md:hidden bg-[#0A0B14]/95 backdrop-blur-md border-t border-white/10 p-4">
          <nav className="flex flex-col gap-4">
            <button onClick={() => { setCurrentPage('home'); setMobileMenuOpen(false); }} className="text-right font-bold text-white hover:text-[#FF6B4A] transition-colors">
              الرئيسية
            </button>
            <button onClick={() => { setCurrentPage('photography'); setMobileMenuOpen(false); }} className="text-right font-bold text-white hover:text-[#FF6B4A] transition-colors">
              التصوير
            </button>
            <button onClick={() => { setCurrentPage('video'); setMobileMenuOpen(false); }} className="text-right font-bold text-white hover:text-[#FF6B4A] transition-colors">
              الفيديو
            </button>
          </nav>
        </div>
      )}
    </header>
  );

  // ==================== FOOTER ====================
  const Footer = () => (
    <footer className="bg-[#0A0B14] border-t border-white/10 py-16 px-4" dir="rtl">
      <div className="container mx-auto">
        <div className="grid md:grid-cols-4 gap-12 mb-12">
          {/* About */}
          <div>
            <h3 className="text-white font-bold text-lg mb-4">عن الشركة</h3>
            <p className="text-[#A0A0A0]">
              نحن متخصصون في إنتاج محتوى بصري احترافي يحقق نتائج قابلة للقياس
            </p>
          </div>

          {/* Quick Links */}
          <div>
            <h3 className="text-white font-bold text-lg mb-4">روابط سريعة</h3>
            <ul className="space-y-2 text-[#A0A0A0]">
              <li><a href="#" className="hover:text-[#FF6B4A] transition-colors">الرئيسية</a></li>
              <li><a href="#" className="hover:text-[#FF6B4A] transition-colors">التصوير</a></li>
              <li><a href="#" className="hover:text-[#FF6B4A] transition-colors">الفيديو</a></li>
              <li><a href="#" className="hover:text-[#FF6B4A] transition-colors">تواصل معنا</a></li>
            </ul>
          </div>

          {/* Services */}
          <div>
            <h3 className="text-white font-bold text-lg mb-4">الخدمات</h3>
            <ul className="space-y-2 text-[#A0A0A0]">
              <li><a href="#" className="hover:text-[#FF6B4A] transition-colors">تصوير المنتجات</a></li>
              <li><a href="#" className="hover:text-[#FF6B4A] transition-colors">إنتاج الفيديو</a></li>
              <li><a href="#" className="hover:text-[#FF6B4A] transition-colors">المونتاج</a></li>
              <li><a href="#" className="hover:text-[#FF6B4A] transition-colors">الرسوميات</a></li>
            </ul>
          </div>

          {/* Contact */}
          <div>
            <h3 className="text-white font-bold text-lg mb-4">تواصل معنا</h3>
            <ul className="space-y-3 text-[#A0A0A0]">
              <li className="flex items-center gap-2">
                <Phone size={18} className="text-[#FF6B4A]" />
                <span>+966 50 123 4567</span>
              </li>
              <li className="flex items-center gap-2">
                <Mail size={18} className="text-[#FF6B4A]" />
                <span>info@optimal.com</span>
              </li>
              <li className="flex items-center gap-2">
                <MapPin size={18} className="text-[#FF6B4A]" />
                <span>الرياض، السعودية</span>
              </li>
            </ul>
          </div>
        </div>

        {/* Newsletter */}
        <div className="bg-[#1A1D2E] border border-white/10 rounded-xl p-8 mb-12">
          <h3 className="text-white font-bold text-xl mb-4">اشترك في النشرة البريدية</h3>
          <div className="flex gap-4">
            <input
              type="email"
              placeholder="بريدك الإلكتروني"
              className="flex-1 bg-[#0A0B14] border border-white/10 rounded-lg px-4 py-3 text-white placeholder-[#A0A0A0] focus:outline-none focus:border-[#FF6B4A]"
            />
            <button className="px-6 py-3 bg-[#FF6B4A] text-white rounded-lg font-bold hover:bg-[#E55A39] transition-colors">
              اشترك
            </button>
          </div>
        </div>

        {/* Social & Copyright */}
        <div className="border-t border-white/10 pt-8 flex flex-col md:flex-row items-center justify-between">
          <p className="text-[#A0A0A0] text-sm">© 2024 الهدف الأمثل للتسويق. جميع الحقوق محفوظة</p>
          <div className="flex gap-4 mt-4 md:mt-0">
            <a href="#" className="text-[#A0A0A0] hover:text-[#FF6B4A] transition-colors">
              <svg className="w-6 h-6" fill="currentColor" viewBox="0 0 24 24"><path d="M23 3a10.9 10.9 0 01-3.14 1.53 4.48 4.48 0 00-7.86 3v1A10.66 10.66 0 013 4s-4 9 5 13a11.64 11.64 0 01-7 2s9 5 20 5a9.5 9.5 0 00-9-5.5c4.75 2.25 7-7 7-7" /></svg>
            </a>
            <a href="#" className="text-[#A0A0A0] hover:text-[#FF6B4A] transition-colors">
              <svg className="w-6 h-6" fill="currentColor" viewBox="0 0 24 24"><rect x="2" y="2" width="20" height="20" rx="5" ry="5" fill="none" stroke="currentColor" strokeWidth="2"/><path d="M16 11.37A4 4 0 1112.63 8 4 4 0 0116 11.37Z" fill="currentColor"/><circle cx="17.5" cy="6.5" r="1.5" fill="currentColor"/></svg>
            </a>
            <a href="#" className="text-[#A0A0A0] hover:text-[#FF6B4A] transition-colors">
              <svg className="w-6 h-6" fill="currentColor" viewBox="0 0 24 24"><path d="M19.615 3.595c-1.42-.82-2.978-1.245-4.61-1.245-4.24 0-7.7 3.46-7.7 7.7 0 1.216.3 2.4.87 3.46l-1.12 4.1 4.2-1.1c1.02.56 2.17.86 3.39.86 4.24 0 7.7-3.46 7.7-7.7 0-2.05-.8-3.98-2.25-5.43z"/></svg>
            </a>
          </div>
        </div>
      </div>
    </footer>
  );

  return (
    <div className={`${darkMode ? 'dark' : ''} min-h-screen bg-[#0A0B14] text-white`}>
      <Header />
      <main className="pt-0">
        {currentPage === 'home' && <HomePage />}
        {currentPage === 'photography' && <PhotographyPage />}
        {currentPage === 'video' && <VideoPage />}
      </main>
      <Footer />
    </div>
  );
}
