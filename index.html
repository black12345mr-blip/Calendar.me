<!DOCTYPE html>
<html lang="th" class="h-full">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>2026 Calendar Web App</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
      /* Custom Scrollbar สำหรับโซนกิจกรรม */
      ::-webkit-scrollbar { width: 4px; height: 4px; }
      ::-webkit-scrollbar-track { background: transparent; }
      ::-webkit-scrollbar-thumb { background: #334155; border-radius: 4px; }
      ::-webkit-scrollbar-thumb:hover { background: #475569; }
    </style>
</head>
<body class="h-full bg-slate-900 text-slate-100 overflow-hidden select-none">

  <!-- App Container (ล็อกไม่ให้จอยืดยาว) -->
  <div class="h-screen w-screen flex overflow-hidden bg-slate-900 text-slate-100">
    
    <!-- Layer 1: Left Sidebar -->
    <aside class="w-64 border-r border-slate-800 flex flex-col shrink-0 p-4 space-y-6 bg-slate-900/50">
      
      <!-- Brand Logo / Title -->
      <div class="flex items-center space-x-3 px-1">
        <div class="w-8 h-8 rounded-xl bg-blue-600 flex items-center justify-center font-bold text-white shadow-lg shadow-blue-500/30">
          26
        </div>
        <span class="font-bold text-lg text-slate-100 tracking-wide">Calendar App</span>
      </div>

      <!-- Create Event Button -->
      <button id="btn-create-event" class="w-full bg-blue-600 hover:bg-blue-500 text-white font-medium py-2.5 px-4 rounded-xl shadow-lg shadow-blue-600/20 transition active:scale-95 flex items-center justify-center space-x-2">
        <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 4v16m8-8H4"></path></svg>
        <span>สร้างกิจกรรม</span>
      </button>

      <!-- Mini Calendar Navigation -->
      <div class="space-y-3 bg-slate-800/40 p-3 rounded-xl border border-slate-800">
        <div class="flex items-center justify-between px-1">
          <span id="mini-month-year" class="text-xs font-bold text-slate-200">มกราคม 2026</span>
          <div class="flex space-x-1">
            <button id="mini-prev" class="p-1 hover:bg-slate-700 rounded-md text-slate-400 hover:text-white transition"><svg class="w-3.5 h-3.5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7"></path></svg></button>
            <button id="mini-next" class="p-1 hover:bg-slate-700 rounded-md text-slate-400 hover:text-white transition"><svg class="w-3.5 h-3.5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"></path></svg></button>
          </div>
        </div>

        <!-- Mini Calendar Grid -->
        <div class="grid grid-cols-7 gap-1 text-center text-[10px] text-slate-400 font-semibold">
          <div class="text-rose-400">อา</div><div>จ</div><div>อ</div><div>พ</div><div>พฤ</div><div>ศ</div><div class="text-blue-400">ส</div>
        </div>
        <div id="mini-calendar-days" class="grid grid-cols-7 gap-1 text-center text-xs">
          <!-- Populated by JS -->
        </div>
      </div>

      <!-- Categories Filter -->
      <div class="flex-1 space-y-3 overflow-y-auto">
        <h3 class="text-xs font-semibold text-slate-400 uppercase tracking-wider px-1">กรองหมวดหมู่</h3>
        <div class="space-y-1">
          <label class="flex items-center space-x-3 px-2 py-1.5 rounded-lg hover:bg-slate-800/60 cursor-pointer transition">
            <input type="checkbox" value="blue" checked class="filter-category rounded border-slate-700 text-blue-500 focus:ring-0 focus:ring-offset-0 bg-slate-800">
            <span class="w-2.5 h-2.5 rounded-full bg-blue-500"></span>
            <span class="text-sm text-slate-300">งานทั่วไป</span>
          </label>
          <label class="flex items-center space-x-3 px-2 py-1.5 rounded-lg hover:bg-slate-800/60 cursor-pointer transition">
            <input type="checkbox" value="purple" checked class="filter-category rounded border-slate-700 text-purple-500 focus:ring-0 focus:ring-offset-0 bg-slate-800">
            <span class="w-2.5 h-2.5 rounded-full bg-purple-500"></span>
            <span class="text-sm text-slate-300">การประชุม</span>
          </label>
          <label class="flex items-center space-x-3 px-2 py-1.5 rounded-lg hover:bg-slate-800/60 cursor-pointer transition">
            <input type="checkbox" value="emerald" checked class="filter-category rounded border-slate-700 text-emerald-500 focus:ring-0 focus:ring-offset-0 bg-slate-800">
            <span class="w-2.5 h-2.5 rounded-full bg-emerald-500"></span>
            <span class="text-sm text-slate-300">ส่วนตัว</span>
          </label>
        </div>
      </div>

    </aside>

    <!-- Main Content Area -->
    <div class="flex-1 flex flex-col h-full overflow-hidden">
      <!-- Top Bar -->
      <header class="h-14 border-b border-slate-800 flex items-center justify-between px-6 shrink-0 bg-slate-900">
        <div class="flex items-center space-x-4">
          <button id="btn-today" class="px-3.5 py-1.5 text-xs font-semibold border border-slate-700 hover:bg-slate-800 rounded-lg text-slate-200 transition">วันนี้</button>
          <div class="flex items-center space-x-1">
            <button id="btn-prev-month" class="p-1.5 hover:bg-slate-800 rounded-lg text-slate-400 hover:text-white transition"><svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7"></path></svg></button>
            <button id="btn-next-month" class="p-1.5 hover:bg-slate-800 rounded-lg text-slate-400 hover:text-white transition"><svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"></path></svg></button>
          </div>
          <h2 id="main-month-title" class="text-xl font-bold text-slate-100 tracking-wide">มกราคม 2026</h2>
        </div>

        <div class="flex items-center space-x-2 bg-slate-800 p-1 rounded-lg border border-slate-700">
          <button class="px-3 py-1 text-xs font-medium rounded-md bg-slate-700 text-white shadow-sm">เดือน</button>
        </div>
      </header>

      <!-- Layer 2: Calendar Grid (มี Internal Scroll เฉพาะจุด) -->
      <main class="flex-1 overflow-y-auto relative flex flex-col">
        <!-- Weekday Header -->
        <div class="grid grid-cols-7 border-b border-slate-800 text-center py-2.5 bg-slate-900/90 sticky top-0 z-10 text-xs font-semibold text-slate-400 uppercase tracking-wider backdrop-blur-sm">
          <div class="text-rose-400">อาทิตย์</div>
          <div>จันทร์</div>
          <div>อังคาร</div>
          <div>พุธ</div>
          <div>พฤหัสบดี</div>
          <div>ศุกร์</div>
          <div class="text-blue-400">เสาร์</div>
        </div>

        <!-- Dynamic Days Grid -->
        <div id="main-calendar-grid" class="flex-1 grid grid-cols-7 auto-rows-fr border-slate-800 min-h-[650px]">
          <!-- Populated by JS -->
        </div>
      </main>
    </div>

    <!-- Backdrop Overlay (สำหรับปิด Drawer เมื่อคลิกด้านนอก) -->
    <div id="drawer-backdrop" class="fixed inset-0 bg-black/50 opacity-0 pointer-events-none transition-opacity duration-300 z-40"></div>

    <!-- Layer 3: Event Detail Drawer (Slide-over) -->
    <aside id="drawer" class="fixed right-0 top-0 h-full w-96 bg-slate-800 border-l border-slate-700 shadow-2xl z-50 transform translate-x-full transition-transform duration-300 ease-in-out flex flex-col">
      <!-- Drawer Header -->
      <div class="h-14 border-b border-slate-700 px-6 flex items-center justify-between">
        <h3 id="drawer-title" class="text-base font-semibold text-slate-100">เพิ่มกิจกรรมใหม่</h3>
        <button id="btn-close-drawer" class="p-1.5 text-slate-400 hover:text-white hover:bg-slate-700 rounded-lg transition">
          <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path></svg>
        </button>
      </div>

      <!-- Drawer Body / Form -->
      <form id="event-form" class="p-6 space-y-4 flex-1 overflow-y-auto">
        <input type="hidden" id="event-id">
        
        <div>
          <label class="block text-xs font-medium text-slate-400 mb-1">ชื่อกิจกรรม <span class="text-rose-400">*</span></label>
          <input type="text" id="event-title" required placeholder="เช่น ประชุมวางแผนงาน Q1" class="w-full bg-slate-900 border border-slate-700 rounded-lg px-3.5 py-2 text-sm text-slate-100 focus:outline-none focus:border-blue-500 transition">
        </div>

        <div class="grid grid-cols-2 gap-3">
          <div>
            <label class="block text-xs font-medium text-slate-400 mb-1">วันที่ <span class="text-rose-400">*</span></label>
            <input type="date" id="event-date" required class="w-full bg-slate-900 border border-slate-700 rounded-lg px-3 py-2 text-sm text-slate-100 focus:outline-none focus:border-blue-500 transition">
          </div>
          <div>
            <label class="block text-xs font-medium text-slate-400 mb-1">เวลา</label>
            <input type="time" id="event-time" value="09:00" class="w-full bg-slate-900 border border-slate-700 rounded-lg px-3 py-2 text-sm text-slate-100 focus:outline-none focus:border-blue-500 transition">
          </div>
        </div>

        <div>
          <label class="block text-xs font-medium text-slate-400 mb-1">หมวดหมู่</label>
          <select id="event-category" class="w-full bg-slate-900 border border-slate-700 rounded-lg px-3 py-2 text-sm text-slate-100 focus:outline-none focus:border-blue-500 transition">
            <option value="blue">งานทั่วไป</option>
            <option value="purple">การประชุม</option>
            <option value="emerald">ส่วนตัว</option>
          </select>
        </div>

        <div>
          <label class="block text-xs font-medium text-slate-400 mb-1">รายละเอียดเพิ่มเติม</label>
          <textarea id="event-desc" rows="4" placeholder="ระบุรายละเอียดเพิ่มเติม..." class="w-full bg-slate-900 border border-slate-700 rounded-lg px-3 py-2 text-sm text-slate-100 focus:outline-none focus:border-blue-500 resize-none transition"></textarea>
        </div>
      </form>

      <!-- Drawer Footer -->
      <div class="p-4 border-t border-slate-700 bg-slate-800/80 flex items-center justify-between">
        <button type="button" id="btn-delete-event" class="px-3 py-2 text-xs font-medium text-rose-400 hover:bg-rose-500/10 rounded-lg transition hidden">ลบกิจกรรม</button>
        <div class="flex items-center space-x-2 ml-auto">
          <button type="button" id="btn-cancel-drawer" class="px-4 py-2 text-xs font-medium text-slate-300 hover:bg-slate-700 rounded-lg transition">ยกเลิก</button>
          <button type="submit" form="event-form" class="px-4 py-2 text-xs font-medium bg-blue-600 hover:bg-blue-500 text-white rounded-lg shadow-md transition">บันทึก</button>
        </div>
      </div>
    </aside>

  </div>

  <!-- Application Logic -->
  <script>
    // Configuration & State
    const thaiMonths = ["มกราคม", "กุมภาพันธ์", "มีนาคม", "เมษายน", "พฤษภาคม", "มิถุนายน", "กรกฎาคม", "สิงหาคม", "กันยายน", "ตลุาคม", "พฤศจิกายน", "ธันวาคม"];
    
    // ตั้งค่าเริ่มต้นเป็น มกราคม 2026
    let currentDate = new Date(2026, 0, 1);
    
    // โหลดข้อมูลกิจกรรมจาก LocalStorage (หากไม่มีจะสร้างข้อมูลเริ่มต้นให้)
    let events = JSON.parse(localStorage.getItem('calendar_events_2026')) || {
      "2026-01-01": [{ id: "1", title: "วันขึ้นปีใหม่ 2026", time: "00:00", category: "emerald", desc: "สวัสดีปีใหม่ 2569" }],
      "2026-01-15": [{ id: "2", title: "ประชุมสรุปแผนงาน Q1", time: "10:00", category: "purple", desc: "เตรียมสไลด์นำเสนอ" }],
      "2026-01-28": [{ id: "3", title: "ส่งรายงานประจำเดือน", time: "17:00", category: "blue", desc: "รวบรวมไฟล์ส่งหัวหน้า" }]
    };

    // DOM Elements
    const mainGrid = document.getElementById("main-calendar-grid");
    const mainMonthTitle = document.getElementById("main-month-title");
    const miniMonthYear = document.getElementById("mini-month-year");
    const miniGrid = document.getElementById("mini-calendar-days");
    const drawer = document.getElementById("drawer");
    const backdrop = document.getElementById("drawer-backdrop");
    const btnDelete = document.getElementById("btn-delete-event");
    const drawerTitle = document.getElementById("drawer-title");

    // Save events to LocalStorage
    function saveEvents() {
      localStorage.setItem('calendar_events_2026', JSON.stringify(events));
    }

    // Filter Active Categories
    function getActiveCategories() {
      const checkboxes = document.querySelectorAll('.filter-category:checked');
      return Array.from(checkboxes).map(cb => cb.value);
    }

    // Main Render Function
    function render() {
      const year = currentDate.getFullYear();
      const month = currentDate.getMonth();

      mainMonthTitle.textContent = `${thaiMonths[month]} ${year}`;
      miniMonthYear.textContent = `${thaiMonths[month]} ${year}`;

      renderMainGrid(year, month);
      renderMiniGrid(year, month);
    }

    // Render Main Grid
    function renderMainGrid(year, month) {
      mainGrid.innerHTML = "";

      const firstDay = new Date(year, month, 1).getDay();
      const totalDays = new Date(year, month + 1, 0).getDate();
      const prevMonthDays = new Date(year, month, 0).getDate();
      const activeCategories = getActiveCategories();

      // Days from previous month
      for (let i = firstDay - 1; i >= 0; i--) {
        const dayNum = prevMonthDays - i;
        const cell = document.createElement("div");
        cell.className = "border-b border-r border-slate-800 p-2 bg-slate-900/40 text-slate-600 text-xs";
        cell.innerHTML = `<span class="font-medium">${dayNum}</span>`;
        mainGrid.appendChild(cell);
      }

      // Current month days
      const realToday = new Date();
      for (let day = 1; day <= totalDays; day++) {
        const dateKey = `${year}-${String(month + 1).padStart(2, '0')}-${String(day).padStart(2, '0')}`;
        const isToday = realToday.getFullYear() === year && realToday.getMonth() === month && realToday.getDate() === day;

        const cell = document.createElement("div");
        cell.className = `border-b border-r border-slate-800 p-2 min-h-[110px] transition hover:bg-slate-800/40 cursor-pointer flex flex-col justify-between group`;
        cell.onclick = (e) => {
          if (!e.target.closest('.event-item')) {
            openDrawerForCreate(dateKey);
          }
        };

        const dayHeader = document.createElement("div");
        dayHeader.className = "flex justify-between items-center";
        
        const daySpan = document.createElement("span");
        daySpan.className = `font-semibold text-xs w-6 h-6 flex items-center justify-center rounded-full ${
          isToday ? "bg-blue-600 text-white shadow-md shadow-blue-500/50" : "text-slate-300 group-hover:text-white"
        }`;
        daySpan.textContent = day;
        dayHeader.appendChild(daySpan);

        cell.appendChild(dayHeader);

        // Events list container
        const eventsContainer = document.createElement("div");
        eventsContainer.className = "mt-1 space-y-1 overflow-y-auto max-h-[85px] flex-1";

        if (events[dateKey]) {
          events[dateKey].forEach(ev => {
            if (!activeCategories.includes(ev.category)) return;

            const evEl = document.createElement("div");
            const colorStyles = {
              blue: "bg-blue-500/15 text-blue-300 border-blue-500/30 hover:bg-blue-500/25",
              purple: "bg-purple-500/15 text-purple-300 border-purple-500/30 hover:bg-purple-500/25",
              emerald: "bg-emerald-500/15 text-emerald-300 border-emerald-500/30 hover:bg-emerald-500/25"
            };

            evEl.className = `event-item text-[11px] p-1.5 rounded border truncate transition cursor-pointer font-medium ${colorStyles[ev.category] || colorStyles.blue}`;
            evEl.textContent = `${ev.time} ${ev.title}`;
            evEl.onclick = (e) => {
              e.stopPropagation();
              openDrawerForEdit(dateKey, ev.id);
            };
            eventsContainer.appendChild(evEl);
          });
        }

        cell.appendChild(eventsContainer);
        mainGrid.appendChild(cell);
      }

      // Fill remaining cells for grid balance
      const totalRendered = firstDay + totalDays;
      const nextDays = (7 - (totalRendered % 7)) % 7;
      for (let i = 1; i <= nextDays; i++) {
        const cell = document.createElement("div");
        cell.className = "border-b border-r border-slate-800 p-2 bg-slate-900/40 text-slate-600 text-xs";
        cell.innerHTML = `<span class="font-medium">${i}</span>`;
        mainGrid.appendChild(cell);
      }
    }

    // Render Sidebar Mini Grid
    function renderMiniGrid(year, month) {
      miniGrid.innerHTML = "";
      const firstDay = new Date(year, month, 1).getDay();
      const totalDays = new Date(year, month + 1, 0).getDate();

      for (let i = 0; i < firstDay; i++) {
        miniGrid.appendChild(document.createElement("div"));
      }

      for (let day = 1; day <= totalDays; day++) {
        const dayEl = document.createElement("button");
        dayEl.className = `w-6 h-6 mx-auto flex items-center justify-center rounded-full hover:bg-slate-700 text-slate-300 text-[11px] transition`;
        dayEl.textContent = day;
        dayEl.onclick = () => {
          const dateKey = `${year}-${String(month + 1).padStart(2, '0')}-${String(day).padStart(2, '0')}`;
          openDrawerForCreate(dateKey);
        };
        miniGrid.appendChild(dayEl);
      }
    }

    // Drawer Management
    function openDrawer() {
      drawer.classList.remove("translate-x-full");
      backdrop.classList.remove("opacity-0", "pointer-events-none");
    }

    function closeDrawer() {
      drawer.classList.add("translate-x-full");
      backdrop.classList.add("opacity-0", "pointer-events-none");
      document.getElementById("event-form").reset();
      document.getElementById("event-id").value = "";
    }

    function openDrawerForCreate(dateStr) {
      drawerTitle.textContent = "เพิ่มกิจกรรมใหม่";
      btnDelete.classList.add("hidden");
      document.getElementById("event-form").reset();
      document.getElementById("event-id").value = "";
      document.getElementById("event-date").value = dateStr;
      openDrawer();
    }

    function openDrawerForEdit(dateStr, eventId) {
      const ev = events[dateStr]?.find(item => item.id === eventId);
      if (!ev) return;

      drawerTitle.textContent = "แก้ไขกิจกรรม";
      btnDelete.classList.remove("hidden");

      document.getElementById("event-id").value = ev.id;
      document.getElementById("event-title").value = ev.title;
      document.getElementById("event-date").value = dateStr;
      document.getElementById("event-time").value = ev.time;
      document.getElementById("event-category").value = ev.category;
      document.getElementById("event-desc").value = ev.desc || "";

      openDrawer();
    }

    // Event Listeners
    document.getElementById("btn-create-event").onclick = () => {
      const year = currentDate.getFullYear();
      const month = String(currentDate.getMonth() + 1).padStart(2, '0');
      openDrawerForCreate(`${year}-${month}-01`);
    };

    document.getElementById("btn-close-drawer").onclick = closeDrawer;
    document.getElementById("btn-cancel-drawer").onclick = closeDrawer;
    backdrop.onclick = closeDrawer;

    // Filter Change Listener
    document.querySelectorAll('.filter-category').forEach(cb => {
      cb.addEventListener('change', render);
    });

    // Navigation Controls
    document.getElementById("btn-prev-month").onclick = () => {
      currentDate.setMonth(currentDate.getMonth() - 1);
      render();
    };

    document.getElementById("btn-next-month").onclick = () => {
      currentDate.setMonth(currentDate.getMonth() + 1);
      render();
    };

    document.getElementById("btn-today").onclick = () => {
      currentDate = new Date(2026, 0, 1);
      render();
    };

    document.getElementById("mini-prev").onclick = () => {
      currentDate.setMonth(currentDate.getMonth() - 1);
      render();
    };

    document.getElementById("mini-next").onclick = () => {
      currentDate.setMonth(currentDate.getMonth() + 1);
      render();
    };

    // Form Submit (Save / Edit)
    document.getElementById("event-form").onsubmit = (e) => {
      e.preventDefault();
      const id = document.getElementById("event-id").value;
      const title = document.getElementById("event-title").value;
      const date = document.getElementById("event-date").value;
      const time = document.getElementById("event-time").value;
      const category = document.getElementById("event-category").value;
      const desc = document.getElementById("event-desc").value;

      // ลบรายการเดิมหากเป็นการแก้ไขหรือย้ายวันที่
      if (id) {
        Object.keys(events).forEach(d => {
          events[d] = events[d].filter(item => item.id !== id);
        });
      }

      if (!events[date]) events[date] = [];
      events[date].push({
        id: id || Date.now().toString(),
        title,
        time,
        category,
        desc
      });

      saveEvents();
      closeDrawer();
      render();
    };

    // Delete Event
    btnDelete.onclick = () => {
      const id = document.getElementById("event-id").value;
      if (!id) return;

      Object.keys(events).forEach(d => {
        events[d] = events[d].filter(item => item.id !== id);
      });

      saveEvents();
      closeDrawer();
      render();
    };

    // Initial Render
    render();
  </script>
</body>
</html>
