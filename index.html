import React, { useState } from 'react';
import { 
  Send, MapPin, Users, Clock, CheckCircle2, 
  ShieldCheck, XCircle, Trash2, Heart, 
  Smartphone, UserCheck, AlertCircle, X
} from 'lucide-react';

export default function App() {
  // Main State
  const [activeTab, setActiveTab] = useState('requester');
  const [requestData, setRequestData] = useState(null);
  const [decision, setDecision] = useState(null); // 'approved' หรือ 'rejected'
  
  // Form State
  const [formData, setFormData] = useState({
    destination: '',
    companions: '',
    returnTime: ''
  });

  // Action: ส่งคำขอ
  const handleSendRequest = (e) => {
    e.preventDefault();
    if (!formData.destination || !formData.companions || !formData.returnTime) return;
    
    setRequestData({ ...formData });
    setDecision(null);
    // สลับไปหน้าคนอนุมัติเพื่อจำลองสถานการณ์
    setActiveTab('approver');
  };

  // Action: อนุมัติ
  const handleApprove = () => {
    setDecision('approved');
  };

  // Action: ไม่อนุมัติ (แบบปกติ ไม่หนี)
  const handleReject = () => {
    setDecision('rejected');
  };

  // Action: เริ่มใหม่
  const handleReset = () => {
    setRequestData(null);
    setDecision(null);
    setFormData({ destination: '', companions: '', returnTime: '' });
    setActiveTab('requester');
  };

  return (
    <div className="min-h-screen bg-slate-50 font-sans p-4 md:p-8 text-slate-900">
      
      {/* Navigation Tabs */}
      <div className="max-w-md mx-auto flex bg-white p-1 rounded-2xl shadow-sm mb-8 border border-slate-200">
        <button 
          onClick={() => setActiveTab('requester')}
          className={`flex-1 flex items-center justify-center py-3 rounded-xl transition-all ${activeTab === 'requester' ? 'bg-blue-600 text-white shadow-md' : 'text-slate-500 hover:bg-slate-50'}`}
        >
          <Smartphone className="w-4 h-4 mr-2" /> ฝั่งแฟน (คนขอ)
        </button>
        <button 
          onClick={() => setActiveTab('approver')}
          className={`flex-1 flex items-center justify-center py-3 rounded-xl transition-all ${activeTab === 'approver' ? 'bg-rose-600 text-white shadow-md' : 'text-slate-500 hover:bg-slate-50'}`}
        >
          <UserCheck className="w-4 h-4 mr-2" /> ฝั่งเรา (คนอนุมัติ)
        </button>
      </div>

      <div className="max-w-md mx-auto">
        {activeTab === 'requester' ? (
          /* --- REQUESTER VIEW --- */
          <div className="bg-white rounded-3xl shadow-xl border border-slate-100 overflow-hidden">
            <div className="bg-blue-600 p-8 text-white text-center">
              <Heart className="mx-auto mb-3 text-blue-200 fill-blue-200" />
              <h1 className="text-2xl font-bold">ใบขออนุญาตไปเที่ยว</h1>
              <p className="text-blue-100 text-sm opacity-90">กรอกรายละเอียดเพื่อส่งคำขอ</p>
            </div>

            <div className="p-8">
              {decision === 'approved' ? (
                <div className="text-center py-6">
                  <div className="w-20 h-20 bg-green-100 rounded-full flex items-center justify-center mx-auto mb-4">
                    <CheckCircle2 className="w-12 h-12 text-green-600" />
                  </div>
                  <h2 className="text-2xl font-bold text-slate-800 mb-2">อนุมัติแล้ว!</h2>
                  <p className="text-slate-500 mb-8 text-sm">เที่ยวให้สนุกนะจ๊ะ อย่าลืมของฝากล่ะ ❤️</p>
                  <div className="inline-block border-8 border-green-600 text-green-600 font-black text-5xl p-3 rotate-[-12deg] rounded-xl uppercase tracking-tighter">
                    APPROVED
                  </div>
                  <button onClick={handleReset} className="block w-full mt-10 text-slate-400 text-xs underline">สร้างใบขอใหม่</button>
                </div>
              ) : decision === 'rejected' ? (
                <div className="text-center py-6">
                  <div className="w-20 h-20 bg-red-100 rounded-full flex items-center justify-center mx-auto mb-4">
                    <X className="w-12 h-12 text-red-600" />
                  </div>
                  <h2 className="text-2xl font-bold text-slate-800 mb-2">ไม่อนุมัติ...</h2>
                  <p className="text-slate-500 mb-8 text-sm">เสียใจด้วยนะ ครั้งนี้อดไปจ้า 🥺</p>
                  <div className="inline-block border-8 border-red-600 text-red-600 font-black text-5xl p-3 rotate-[12deg] rounded-xl uppercase tracking-tighter">
                    REJECTED
                  </div>
                  <button onClick={handleReset} className="block w-full mt-10 text-slate-400 text-xs underline">ลองขอใหม่อีกครั้ง</button>
                </div>
              ) : requestData ? (
                <div className="text-center py-12">
                  <div className="bg-blue-50 p-6 rounded-full inline-block mb-6">
                    <Send className="w-10 h-10 text-blue-600 animate-pulse" />
                  </div>
                  <h3 className="text-xl font-bold text-slate-800">ส่งคำขอแล้ว</h3>
                  <p className="text-slate-500 text-sm mt-2 italic">กำลังรอการพิจารณา...</p>
                </div>
              ) : (
                <form onSubmit={handleSendRequest} className="space-y-5">
                  <div className="space-y-2">
                    <label className="text-sm font-bold text-slate-600 flex items-center">
                      <MapPin className="w-4 h-4 mr-2 text-blue-500" /> สถานที่:
                    </label>
                    <input 
                      required
                      className="w-full bg-slate-50 border border-slate-200 rounded-xl p-4 outline-none focus:border-blue-500 transition-all"
                      placeholder="เช่น สยาม, บ้านเพื่อน"
                      value={formData.destination}
                      onChange={e => setFormData({...formData, destination: e.target.value})}
                    />
                  </div>
                  <div className="space-y-2">
                    <label className="text-sm font-bold text-slate-600 flex items-center">
                      <Users className="w-4 h-4 mr-2 text-blue-500" /> ไปกับใคร:
                    </label>
                    <input 
                      required
                      className="w-full bg-slate-50 border border-slate-200 rounded-xl p-4 outline-none focus:border-blue-500 transition-all"
                      placeholder="ระบุชื่อเพื่อน..."
                      value={formData.companions}
                      onChange={e => setFormData({...formData, companions: e.target.value})}
                    />
                  </div>
                  <div className="space-y-2">
                    <label className="text-sm font-bold text-slate-600 flex items-center">
                      <Clock className="w-4 h-4 mr-2 text-blue-500" /> เวลากลับ:
                    </label>
                    <input 
                      required
                      type="time"
                      className="w-full bg-slate-50 border border-slate-200 rounded-xl p-4 outline-none focus:border-blue-500 transition-all"
                      value={formData.returnTime}
                      onChange={e => setFormData({...formData, returnTime: e.target.value})}
                    />
                  </div>
                  <button 
                    type="submit"
                    className="w-full bg-blue-600 hover:bg-blue-700 text-white font-bold py-4 rounded-xl shadow-lg transform active:scale-95 transition-all"
                  >
                    ส่งใบขออนุญาต 💌
                  </button>
                </form>
              )}
            </div>
          </div>
        ) : (
          /* --- APPROVER VIEW --- */
          <div className="bg-white rounded-3xl shadow-xl border border-slate-100 overflow-hidden">
            <div className="bg-rose-500 p-8 text-white flex justify-between items-center">
              <div>
                <h2 className="text-2xl font-bold">ผู้อนุมัติ</h2>
                <p className="text-rose-100 text-sm opacity-90">ตรวจสอบและตัดสินใจ</p>
              </div>
              {requestData && (
                <button onClick={handleReset} className="p-2 hover:bg-rose-600 rounded-lg text-rose-100">
                  <Trash2 className="w-5 h-5" />
                </button>
              )}
            </div>

            <div className="p-8">
              {!requestData ? (
                <div className="text-center py-16 text-slate-300">
                  <AlertCircle className="w-16 h-16 mx-auto mb-4 opacity-20" />
                  <p className="italic">ยังไม่มีคำขอส่งเข้ามา</p>
                </div>
              ) : decision ? (
                <div className="text-center py-10">
                  <div className={`border-8 ${decision === 'approved' ? 'border-green-600 text-green-600' : 'border-red-600 text-red-600'} font-black text-5xl p-4 rotate-[-12deg] inline-block mb-8 rounded-xl`}>
                    {decision === 'approved' ? 'APPROVED' : 'REJECTED'}
                  </div>
                  <p className="text-slate-600 italic">ทำรายการเรียบร้อยแล้ว</p>
                </div>
              ) : (
                <div className="space-y-6">
                  <div className="bg-slate-50 rounded-2xl p-6 border border-slate-100 space-y-4 shadow-inner">
                    <div className="flex items-center">
                      <MapPin className="w-5 h-5 mr-3 text-rose-500" />
                      <p className="text-slate-700"><strong>ที่ไหน:</strong> {requestData.destination}</p>
                    </div>
                    <div className="flex items-center">
                      <Users className="w-5 h-5 mr-3 text-rose-500" />
                      <p className="text-slate-700"><strong>ใครบ้าง:</strong> {requestData.companions}</p>
                    </div>
                    <div className="flex items-center">
                      <Clock className="w-5 h-5 mr-3 text-rose-500" />
                      <p className="text-slate-700"><strong>กลับ:</strong> {requestData.returnTime} น.</p>
                    </div>
                  </div>

                  <div className="space-y-3">
                    <button 
                      onClick={handleApprove}
                      className="w-full bg-green-500 hover:bg-green-600 text-white font-bold py-4 rounded-xl shadow-lg flex items-center justify-center space-x-2 transform active:scale-95 transition-all"
                    >
                      <ShieldCheck className="w-6 h-6" />
                      <span>อนุมัติให้ไป ✅</span>
                    </button>
                    
                    <button 
                      onClick={handleReject}
                      className="w-full bg-red-500 hover:bg-red-600 text-white font-bold py-4 rounded-xl shadow-lg flex items-center justify-center space-x-2 transform active:scale-95 transition-all"
                    >
                      <XCircle className="w-6 h-6" />
                      <span>ไม่อนุมัติ ❌</span>
                    </button>
                  </div>
                </div>
              )}
            </div>
          </div>
        )}
      </div>
    </div>
  );
}
