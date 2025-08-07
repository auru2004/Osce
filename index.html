<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="utf-8"/>
    <meta name="viewport" content="width=device-width, initial-scale=1"/>
    <title>Stopwatch OSCE - Professional Timer</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet"/>
    <style>
        :root {
            --primary-blue: #2563eb;
            --primary-purple: #7c3aed;
            --accent-cyan: #06b6d4;
            --accent-emerald: #10b981;
            --accent-amber: #f59e0b;
            --accent-rose: #f43f5e;
            --dark-slate: #0f172a;
            --light-slate: #f1f5f9;
        }

        * {
            scrollbar-width: thin;
            scrollbar-color: var(--primary-blue) #e2e8f0;
        }

        *::-webkit-scrollbar {
            width: 6px;
        }

        *::-webkit-scrollbar-track {
            background: #f1f5f9;
            border-radius: 3px;
        }

        *::-webkit-scrollbar-thumb {
            background: var(--primary-blue);
            border-radius: 3px;
        }

        body {
            font-family: "Inter", sans-serif;
            background: linear-gradient(135deg, #0f172a 0%, #1e293b 25%, #334155 50%, #475569 75%, #64748b 100%);
            min-height: 100vh;
            position: relative;
            overflow-x: hidden;
        }

        body::before {
            content: '';
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: radial-gradient(circle at 20% 50%, rgba(37, 99, 235, 0.1) 0%, transparent 50%),
                        radial-gradient(circle at 80% 20%, rgba(124, 58, 237, 0.1) 0%, transparent 50%),
                        radial-gradient(circle at 40% 80%, rgba(6, 182, 212, 0.1) 0%, transparent 50%);
            pointer-events: none;
            z-index: 0;
        }

        .main-container {
            position: relative;
            z-index: 1;
        }

        /* Tutorial Styles */
        .tutorial-overlay {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(135deg, #0f172a 0%, #1e293b 25%, #334155 50%, #475569 75%, #64748b 100%);
            z-index: 2000;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.5s ease;
        }

        .tutorial-overlay.hidden {
            opacity: 0;
            visibility: hidden;
            transform: translateY(-100%);
        }

        .tutorial-container {
            max-width: 1000px;
            width: 90%;
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(20px);
            border: 1px solid rgba(255, 255, 255, 0.2);
            border-radius: 24px;
            padding: 40px;
            text-align: center;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
        }

        .tutorial-header {
            margin-bottom: 32px;
        }

        .tutorial-title {
            font-size: 2.5rem;
            font-weight: 800;
            color: #ffffff;
            margin-bottom: 12px;
            background: linear-gradient(135deg, #3b82f6 0%, #8b5cf6 50%, #06b6d4 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .tutorial-subtitle {
            font-size: 1.2rem;
            color: rgba(255, 255, 255, 0.8);
            margin-bottom: 8px;
        }

        .tutorial-description {
            font-size: 1rem;
            color: rgba(255, 255, 255, 0.6);
        }

        .slider-container {
            position: relative;
            margin-bottom: 32px;
        }

        .slider-wrapper {
            overflow: hidden;
            border-radius: 16px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
        }

        .slider-track {
            display: flex;
            transition: transform 0.5s ease;
        }

        .slide {
            min-width: 100%;
            position: relative;
        }

        .slide img {
            width: 100%;
            height: 400px;
            object-fit: cover;
            border-radius: 16px;
        }

        .slide-caption {
            position: absolute;
            bottom: 0;
            left: 0;
            right: 0;
            background: linear-gradient(transparent, rgba(0, 0, 0, 0.8));
            color: white;
            padding: 24px;
            border-radius: 0 0 16px 16px;
        }

        .slide-caption h3 {
            font-size: 1.25rem;
            font-weight: 600;
            margin-bottom: 8px;
        }

        .slide-caption p {
            font-size: 0.9rem;
            opacity: 0.9;
            line-height: 1.4;
        }

 .slider-nav {
    background: transparent;
    border: none;
    color: white; /* atau ganti sesuai warna yang kamu mau */
    font-size: 1.5rem;
    cursor: pointer;
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    width: 48px;
    height: 48px;
    display: flex;
    align-items: center;
    justify-content: center;
    transition: all 0.3s ease;
}


        .slider-nav:hover {
            background: rgba(255, 255, 255, 0.3);
            transform: translateY(-50%) scale(1.1);
        }

        .slider-nav.prev {
            left: 16px;
        }

        .slider-nav.next {
            right: 16px;
        }

        .slider-nav.disabled {
            opacity: 0.3;
            cursor: not-allowed;
        }

        .slider-nav.disabled:hover {
            transform: translateY(-50%) scale(1);
            background: rgba(255, 255, 255, 0.2);
        }

        .slider-dots {
            display: flex;
            justify-content: center;
            gap: 12px;
            margin-top: 24px;
        }

        .dot {
            width: 12px;
            height: 12px;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.3);
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .dot.active {
            background: var(--primary-blue);
            transform: scale(1.2);
        }

        .slide-counter {
            color: rgba(255, 255, 255, 0.7);
            font-size: 0.9rem;
            margin-bottom: 16px;
        }

        .tutorial-actions {
            display: flex;
            justify-content: center;
            gap: 16px;
            margin-top: 32px;
        }

        .btn-tutorial {
            padding: 14px 32px;
            border-radius: 12px;
            font-weight: 600;
            font-size: 1rem;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        .btn-start {
            background: linear-gradient(135deg, var(--accent-emerald) 0%, #059669 100%);
            color: white;
            box-shadow: 0 4px 15px rgba(16, 185, 129, 0.3);
        }

        .btn-start:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 25px rgba(16, 185, 129, 0.4);
        }

        .btn-skip {
            background: rgba(255, 255, 255, 0.1);
            color: rgba(255, 255, 255, 0.8);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        .btn-skip:hover {
            background: rgba(255, 255, 255, 0.2);
            color: white;
        }

        .glass-card {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(20px);
            border: 1px solid rgba(255, 255, 255, 0.2);
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.1);
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
            overflow: hidden;
        }

        .glass-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.1), transparent);
            transition: left 0.6s;
        }

        .glass-card:hover::before {
            left: 100%;
        }

        .glass-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.15);
            border-color: rgba(255, 255, 255, 0.3);
        }

        .timer-display {
            font-size: 4rem;
            font-weight: 800;
            color: #ffffff;
            text-align: center;
            letter-spacing: 0.1em;
            font-feature-settings: "tnum";
            background: linear-gradient(135deg, #3b82f6 0%, #8b5cf6 50%, #06b6d4 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            text-shadow: 0 0 40px rgba(59, 130, 246, 0.5);
            transition: all 0.3s ease;
            position: relative;
        }

        .timer-active {
            animation: pulse-glow 2s ease-in-out infinite alternate;
        }

        @keyframes pulse-glow {
            from {
                text-shadow: 0 0 20px rgba(59, 130, 246, 0.5), 0 0 40px rgba(139, 92, 246, 0.3);
                transform: scale(1);
            }
            to {
                text-shadow: 0 0 30px rgba(59, 130, 246, 0.8), 0 0 60px rgba(139, 92, 246, 0.5);
                transform: scale(1.02);
            }
        }

        .btn-primary {
            background: linear-gradient(135deg, var(--primary-blue) 0%, var(--primary-purple) 100%);
            color: white;
            border: none;
            padding: 14px 28px;
            border-radius: 12px;
            font-weight: 600;
            font-size: 0.95rem;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(37, 99, 235, 0.3);
            position: relative;
            overflow: hidden;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        .btn-primary::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            transition: left 0.6s;
        }

        .btn-primary:hover::before {
            left: 100%;
        }

        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 25px rgba(37, 99, 235, 0.4);
        }

        .btn-primary:active {
            transform: translateY(0);
        }

        .btn-secondary {
            background: linear-gradient(135deg, #64748b 0%, #475569 100%);
            color: white;
            border: none;
            padding: 14px 28px;
            border-radius: 12px;
            font-weight: 600;
            font-size: 0.95rem;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(100, 116, 139, 0.3);
            position: relative;
            overflow: hidden;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        .btn-secondary::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            transition: left 0.6s;
        }

        .btn-secondary:hover::before {
            left: 100%;
        }

        .btn-secondary:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 25px rgba(100, 116, 139, 0.4);
        }

        .btn-success {
            background: linear-gradient(135deg, var(--accent-emerald) 0%, #059669 100%);
            color: white;
            border: none;
            padding: 14px 28px;
            border-radius: 12px;
            font-weight: 600;
            font-size: 0.95rem;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(16, 185, 129, 0.3);
            position: relative;
            overflow: hidden;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        .btn-success::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            transition: left 0.6s;
        }

        .btn-success:hover::before {
            left: 100%;
        }

        .btn-success:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 25px rgba(16, 185, 129, 0.4);
        }

        .btn-danger {
            background: linear-gradient(135deg, var(--accent-rose) 0%, #e11d48 100%);
            color: white;
            border: none;
            padding: 10px 18px;
            border-radius: 8px;
            font-weight: 600;
            transition: all 0.3s ease;
            font-size: 0.875rem;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        .btn-danger:hover {
            transform: translateY(-1px);
            box-shadow: 0 6px 20px rgba(244, 63, 94, 0.4);
        }

        .btn-edit {
            background: linear-gradient(135deg, var(--accent-amber) 0%, #d97706 100%);
            color: white;
            border: none;
            padding: 10px 18px;
            border-radius: 8px;
            font-weight: 600;
            transition: all 0.3s ease;
            font-size: 0.875rem;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        .btn-edit:hover {
            transform: translateY(-1px);
            box-shadow: 0 6px 20px rgba(245, 158, 11, 0.4);
        }

        .btn-duplicate {
            background: linear-gradient(135deg, var(--accent-cyan) 0%, #0891b2 100%);
            color: white;
            border: none;
            padding: 10px 18px;
            border-radius: 8px;
            font-weight: 600;
            transition: all 0.3s ease;
            font-size: 0.875rem;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        .btn-duplicate:hover {
            transform: translateY(-1px);
            box-shadow: 0 6px 20px rgba(6, 182, 212, 0.4);
        }

        .input-field {
            border: 2px solid rgba(255, 255, 255, 0.2);
            border-radius: 12px;
            padding: 14px 18px;
            font-size: 1rem;
            transition: all 0.3s ease;
            background: rgba(255, 255, 255, 0.1);
            color: #ffffff;
            backdrop-filter: blur(10px);
        }

        .input-field::placeholder {
            color: rgba(255, 255, 255, 0.6);
        }

        .input-field:focus {
            outline: none;
            border-color: var(--primary-blue);
            box-shadow: 0 0 0 4px rgba(37, 99, 235, 0.2);
            background: rgba(255, 255, 255, 0.15);
        }

        .select-field {
            border: 2px solid rgba(255, 255, 255, 0.2);
            border-radius: 12px;
            padding: 14px 18px;
            font-size: 1rem;
            transition: all 0.3s ease;
            background: rgba(255, 255, 255, 0.1);
            color: #ffffff;
            backdrop-filter: blur(10px);
            appearance: none;
            background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' fill='none' viewBox='0 0 20 20'%3e%3cpath stroke='%23ffffff' stroke-linecap='round' stroke-linejoin='round' stroke-width='1.5' d='m6 8 4 4 4-4'/%3e%3c/svg%3e");
            background-position: right 12px center;
            background-repeat: no-repeat;
            background-size: 16px;
            padding-right: 40px;
        }

        .select-field:focus {
            outline: none;
            border-color: var(--primary-blue);
            box-shadow: 0 0 0 4px rgba(37, 99, 235, 0.2);
            background: rgba(255, 255, 255, 0.15);
        }

        .select-field option {
            background: #1e293b;
            color: #ffffff;
        }

        .progress-bar {
            height: 8px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 4px;
            overflow: hidden;
            margin: 24px 0;
            backdrop-filter: blur(10px);
        }

        .progress-fill {
            height: 100%;
            background: linear-gradient(90deg, var(--primary-blue) 0%, var(--primary-purple) 50%, var(--accent-cyan) 100%);
            border-radius: 4px;
            transition: width 0.5s ease;
            box-shadow: 0 0 20px rgba(59, 130, 246, 0.5);
            animation: shimmer 2s infinite;
        }

        @keyframes shimmer {
            0% { background-position: -200px 0; }
            100% { background-position: 200px 0; }
        }

        .message-item {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(15px);
            border: 1px solid rgba(255, 255, 255, 0.2);
            border-radius: 16px;
            padding: 20px;
            margin-bottom: 16px;
            transition: all 0.3s ease;
            border-left: 4px solid var(--primary-blue);
            position: relative;
            overflow: hidden;
        }

        .message-item::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.1), transparent);
            transition: left 0.6s;
        }

        .message-item:hover::before {
            left: 100%;
        }

        .message-item:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.15);
            border-color: rgba(255, 255, 255, 0.3);
        }

        .message-item.active {
            background: rgba(16, 185, 129, 0.2);
            border-left-color: var(--accent-emerald);
            animation: pulse-border 1s ease-in-out infinite alternate;
        }

        @keyframes pulse-border {
            from { border-left-color: var(--accent-emerald); }
            to { border-left-color: #059669; }
        }

        .fade-in {
            animation: fadeIn 0.6s ease-out;
        }

        @keyframes fadeIn {
            from {
                opacity: 0;
                transform: translateY(20px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .slide-in {
            animation: slideIn 0.4s ease-out;
        }

        @keyframes slideIn {
            from {
                transform: translateX(-20px);
                opacity: 0;
            }
            to {
                transform: translateX(0);
                opacity: 1;
            }
        }

        .notification {
            position: fixed;
            top: 20px;
            right: 20px;
            padding: 18px 24px;
            border-radius: 12px;
            color: white;
            font-weight: 600;
            z-index: 1000;
            animation: slideInRight 0.4s ease-out;
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.2);
            backdrop-filter: blur(10px);
        }

        @keyframes slideInRight {
            from {
                transform: translateX(100%);
                opacity: 0;
            }
            to {
                transform: translateX(0);
                opacity: 1;
            }
        }

        .notification.success {
            background: linear-gradient(135deg, var(--accent-emerald) 0%, #059669 100%);
        }

        .notification.error {
            background: linear-gradient(135deg, var(--accent-rose) 0%, #e11d48 100%);
        }

        .notification.info {
            background: linear-gradient(135deg, var(--primary-blue) 0%, var(--primary-purple) 100%);
        }

        .status-badge {
            display: inline-flex;
            align-items: center;
            padding: 6px 12px;
            border-radius: 20px;
            font-size: 0.75rem;
            font-weight: 600;
            gap: 6px;
            text-transform: uppercase;
            letter-spacing: 0.5px;
        }

        .status-badge.pending {
            background: rgba(37, 99, 235, 0.2);
            color: #60a5fa;
            border: 1px solid rgba(37, 99, 235, 0.3);
        }

        .status-badge.active {
            background: rgba(16, 185, 129, 0.2);
            color: #34d399;
            border: 1px solid rgba(16, 185, 129, 0.3);
        }

        .status-badge.completed {
            background: rgba(139, 92, 246, 0.2);
            color: #a78bfa;
            border: 1px solid rgba(139, 92, 246, 0.3);
        }

        .empty-state {
            text-align: center;
            padding: 60px 20px;
            color: rgba(255, 255, 255, 0.6);
        }

        .empty-state .icon {
            font-size: 4rem;
            margin-bottom: 20px;
            opacity: 0.7;
        }

        .floating-particles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 0;
        }

        .particle {
            position: absolute;
            width: 4px;
            height: 4px;
            background: rgba(255, 255, 255, 0.3);
            border-radius: 50%;
            animation: float 20s infinite linear;
        }

        @keyframes float {
            0% {
                transform: translateY(100vh) rotate(0deg);
                opacity: 0;
            }
            10% {
                opacity: 1;
            }
            90% {
                opacity: 1;
            }
            100% {
                transform: translateY(-100vh) rotate(360deg);
                opacity: 0;
            }
        }

        .header-glow {
            position: relative;
        }

        .header-glow::before {
            content: '';
            position: absolute;
            top: 50%;
            left: 50%;
            width: 100px;
            height: 100px;
            background: radial-gradient(circle, rgba(59, 130, 246, 0.3) 0%, transparent 70%);
            border-radius: 50%;
            transform: translate(-50%, -50%);
            animation: pulse 2s ease-in-out infinite alternate;
        }

        @keyframes pulse {
            0% {
                transform: translate(-50%, -50%) scale(1);
            }
            100% {
                transform: translate(-50%, -50%) scale(1.2);
            }
        }

        /* Modal Styles */
        .modal-overlay {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(0, 0, 0, 0.7);
            backdrop-filter: blur(8px);
            z-index: 1000;
            display: flex;
            align-items: center;
            justify-content: center;
            opacity: 0;
            visibility: hidden;
            transition: all 0.3s ease;
        }

        .modal-overlay.active {
            opacity: 1;
            visibility: visible;
        }

        .modal-content {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(20px);
            border: 1px solid rgba(255, 255, 255, 0.2);
            border-radius: 20px;
            padding: 32px;
            max-width: 500px;
            width: 90%;
            max-height: 80vh;
            overflow-y: auto;
            transform: scale(0.9) translateY(20px);
            transition: all 0.3s ease;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
        }

        .modal-overlay.active .modal-content {
            transform: scale(1) translateY(0);
        }

        .modal-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 24px;
            padding-bottom: 16px;
            border-bottom: 1px solid rgba(255, 255, 255, 0.2);
        }

        .modal-title {
            font-size: 1.5rem;
            font-weight: 700;
            color: #ffffff;
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .modal-close {
            background: rgba(255, 255, 255, 0.1);
            border: 1px solid rgba(255, 255, 255, 0.2);
            border-radius: 8px;
            width: 40px;
            height: 40px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: #ffffff;
            font-size: 1.2rem;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .modal-close:hover {
            background: rgba(255, 255, 255, 0.2);
            transform: scale(1.1);
        }

        /* Profile Section Styles */
        .profile-section {
            background: linear-gradient(135deg, rgba(16, 185, 129, 0.05) 0%, rgba(6, 182, 212, 0.05) 100%);
            border: 1px solid rgba(16, 185, 129, 0.2);
        }

        .profile-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 24px;
            margin-top: 24px;
        }

        .profile-card {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(15px);
            border: 1px solid rgba(255, 255, 255, 0.2);
            border-radius: 20px;
            padding: 24px;
            transition: all 0.4s ease;
            cursor: pointer;
            position: relative;
            overflow: hidden;
            text-decoration: none;
            color: inherit;
        }

        .profile-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.1), transparent);
            transition: left 0.6s;
        }

        .profile-card:hover::before {
            left: 100%;
        }

        .profile-card:hover {
            transform: translateY(-8px) scale(1.02);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.2);
            border-color: rgba(16, 185, 129, 0.4);
        }

        .profile-image {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            object-fit: cover;
            margin: 0 auto 20px;
            border: 4px solid rgba(16, 185, 129, 0.3);
            transition: all 0.3s ease;
        }

        .profile-card:hover .profile-image {
            border-color: rgba(16, 185, 129, 0.6);
            transform: scale(1.05);
        }

        .profile-name {
            font-size: 1.25rem;
            font-weight: 700;
            color: #ffffff;
            margin-bottom: 8px;
            text-align: center;
        }

        .profile-role {
            font-size: 1rem;
            font-weight: 600;
            color: rgba(16, 185, 129, 0.9);
            margin-bottom: 12px;
            text-align: center;
        }

        .profile-description {
            font-size: 0.9rem;
            color: rgba(255, 255, 255, 0.8);
            line-height: 1.5;
            text-align: center;
        }

        .profile-link-icon {
            position: absolute;
            top: 16px;
            right: 16px;
            width: 24px;
            height: 24px;
            background: rgba(16, 185, 129, 0.2);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: rgba(16, 185, 129, 0.8);
            font-size: 12px;
            transition: all 0.3s ease;
        }

        .profile-card:hover .profile-link-icon {
            background: rgba(16, 185, 129, 0.3);
            color: rgba(16, 185, 129, 1);
            transform: scale(1.1);
        }

        @media (max-width: 768px) {
            .timer-display {
                font-size: 2.5rem;
            }
            .notification {
                left: 20px;
                right: 20px;
            }
            .modal-content {
                padding: 24px;
                margin: 20px;
            }
            .tutorial-container {
                padding: 24px;
                margin: 20px;
            }
            .tutorial-title {
                font-size: 2rem;
            }
            .slide img {
                height: 300px;
            }
            .slider-nav {
                width: 40px;
                height: 40px;
            }
            .profile-grid {
                grid-template-columns: 1fr;
                gap: 16px;
            }
            .profile-card {
                padding: 20px;
            }
            .profile-image {
                width: 100px;
                height: 100px;
            }
        }

        .voice-preview {
            display: flex;
            align-items: center;
            gap: 8px;
            margin-top: 8px;
        }

        .voice-preview button {
            padding: 6px 12px;
            border: 1px solid rgba(255, 255, 255, 0.3);
            border-radius: 8px;
            background: rgba(255, 255, 255, 0.1);
            color: #ffffff;
            font-size: 0.75rem;
            transition: all 0.3s ease;
        }

        .voice-preview button:hover {
            background: rgba(255, 255, 255, 0.2);
            transform: translateY(-1px);
        }

        .bell-preview {
            display: flex;
            align-items: center;
            gap: 8px;
            margin-top: 8px;
        }

        .bell-preview button {
            padding: 6px 12px;
            border: 1px solid rgba(255, 255, 255, 0.3);
            border-radius: 8px;
            background: rgba(255, 255, 255, 0.1);
            color: #ffffff;
            font-size: 0.75rem;
            transition: all 0.3s ease;
        }

        .bell-preview button:hover {
            background: rgba(255, 255, 255, 0.2);
            transform: translateY(-1px);
        }
    </style>
</head>
<body class="min-h-screen p-4">
    <!-- Tutorial Overlay -->
    <div class="tutorial-overlay" id="tutorialOverlay">
        <div class="tutorial-container">
            <div class="tutorial-header">
                <h1 class="tutorial-title">Tutorial Penggunaan</h1>
                <p class="tutorial-subtitle">Stopwatch OSCE - Professional Timer</p>
                <p class="tutorial-description">Pelajari cara menggunakan aplikasi timer OSCE dengan mudah</p>
            </div>

            <div class="slider-container">
                <div class="slide-counter">
                    <span id="currentSlide">1</span> / <span id="totalSlides">15</span>
                </div>
                
                <div class="slider-wrapper">
                    <div class="slider-track" id="sliderTrack">
                        <!-- Slide 1 -->
                        <div class="slide">
                            <img src="gambar1.jpg" alt="Tutorial 1">
                            <div class="slide-caption">
                                <h3>Selamat Datang di OSCE Timer</h3>
                                <p>Aplikasi profesional untuk mengatur waktu ujian OSCE dengan fitur pesan suara otomatis dan pengaturan yang fleksibel.</p>
                            </div>
                        </div>

                        <!-- Slide 2 -->
                        <div class="slide">
                            <img src="gambar2.jpg" alt="Tutorial 2">
                            <div class="slide-caption">
                                <h3></h3>
                                <p></p>
                            </div>
                        </div>

                        <!-- Slide 3 -->
                        <div class="slide">
                            <img src="gambar3.jpg" alt="Tutorial 3">
                            <div class="slide-caption">
                                <h3></h3>
                                <p></p>
                            </div>
                        </div>

                        <!-- Slide 4 -->
                        <div class="slide">
                            <img src="gambar4.jpg" alt="Tutorial 4">
                            <div class="slide-caption">
                                <h3></h3>
                                <p></p>
                            </div>
                        </div>

                        <!-- Slide 5 -->
                        <div class="slide">
                            <img src="gambar5.jpg" alt="Tutorial 5">
                            <div class="slide-caption">
                                <h3></h3>
                                <p></p>
                            </div>
                        </div>

                        <!-- Slide 6 -->
                        <div class="slide">
                            <img src="gambar6.jpg" alt="Tutorial 6">
                            <div class="slide-caption">
                                <h3></h3>
                                <p></p>
                            </div>
                        </div>

                        <!-- Slide 7 -->
                        <div class="slide">
                            <img src="gambar7.jpg" alt="Tutorial 7">
                            <div class="slide-caption">
                                <h3></h3>
                                <p></p>
                            </div>
                        </div>

                        <!-- Slide 8 -->
                        <div class="slide">
                            <img src="gambar8.jpg" alt="Tutorial 8">
                            <div class="slide-caption">
                                <h3></h3>
                                <p></p>
                            </div>
                        </div>

                        <!-- Slide 9 -->
                        <div class="slide">
                            <img src="gambar9.jpg" alt="Tutorial 9">
                            <div class="slide-caption">
                                <h3></h3>
                                <p></p>
                            </div>
                        </div>

                        <!-- Slide 10 -->
                        <div class="slide">
                            <img src="gambar10.jpg" alt="Tutorial 10">
                            <div class="slide-caption">
                                <h3></h3>
                                <p></p>
                            </div>
                        </div>

                        <!-- Slide 11 -->
                        <div class="slide">
                            <img src="gambar11.jpg" alt="Tutorial 11">
                            <div class="slide-caption">
                                <h3></h3>
                                <p></p>
                            </div>
                        </div>

                        <!-- Slide 12 -->
                        <div class="slide">
                            <img src="gambar12.jpg" alt="Tutorial 12">
                            <div class="slide-caption">
                                <h3></h3>
                                <p></p>
                            </div>
                        </div>

                        <!-- Slide 13 -->
                        <div class="slide">
                            <img src="gambar13.jpg" alt="Tutorial 13">
                            <div class="slide-caption">
                                <h3></h3>
                                <p></p>
                            </div>
                        </div>

                        <!-- Slide 14 -->
                        <div class="slide">
                            <img src="gambar14.jpg" alt="Tutorial 14">
                            <div class="slide-caption">
                                <h3></h3>
                                <p></p>
                            </div>
                        </div>

                        <!-- Slide 15 -->
                        <div class="slide">
                            <img src="gambar15.jpg" alt="Tutorial 15">
                            <div class="slide-caption">
                                <h3></h3>
                                <p></p>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Navigation Buttons -->
                <button class="slider-nav prev" id="prevBtn" onclick="previousSlide()">‹</button>
                <button class="slider-nav next" id="nextBtn" onclick="nextSlide()">›</button>

                <!-- Dots Indicator -->
                <div class="slider-dots" id="sliderDots"></div>
            </div>

            <div class="tutorial-actions">
                <button class="btn-tutorial btn-skip" onclick="skipTutorial()">
                    ⏭️ Lewati Tutorial
                </button>
                <button class="btn-tutorial btn-start" id="startBtn" onclick="startApp()" style="display: none;">
                    🚀 Mulai Aplikasi
                </button>
            </div>
        </div>
    </div>

    <!-- Floating Particles -->
    <div class="floating-particles" id="particles"></div>

    <!-- Edit Modal -->
    <div class="modal-overlay" id="editModal">
        <div class="modal-content">
            <div class="modal-header">
                <h3 class="modal-title">
                    <span>✏️</span>
                    Edit Pesan
                </h3>
                <button class="modal-close" onclick="closeEditModal()">×</button>
            </div>
            <div class="space-y-6">
                <div>
                    <label class="block text-sm font-semibold text-gray-300 mb-3">Pesan</label>
                    <textarea id="editMessageText" rows="3" placeholder="Masukkan pesan yang akan diucapkan..." class="input-field w-full resize-none"></textarea>
                </div>
                <div class="grid grid-cols-2 gap-4">
                    <div>
                        <label class="block text-sm font-semibold text-gray-300 mb-3">Menit</label>
                        <input id="editMessageMinute" type="number" min="0" max="60" value="0" class="input-field w-full">
                    </div>
                    <div>
                        <label class="block text-sm font-semibold text-gray-300 mb-3">Detik</label>
                        <input id="editMessageSecond" type="number" min="0" max="59" value="10" class="input-field w-full">
                    </div>
                </div>
                <div class="grid grid-cols-2 gap-4">
                    <button id="updateMessageBtn" class="btn-success w-full">
                        🔄 Update Pesan
                    </button>
                    <button id="testEditMessageBtn" class="btn-primary w-full">
                        🎤 Test Pesan
                    </button>
                </div>
            </div>
        </div>
    </div>

    <div class="main-container max-w-6xl mx-auto">
        <!-- Header -->
        <div class="text-center mb-8 fade-in">
            <div class="header-glow inline-flex items-center justify-center w-20 h-20 bg-gradient-to-r from-blue-500 to-purple-600 rounded-full mb-6 relative">
                <svg class="w-10 h-10 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z"></path>
                </svg>
            </div>
            <h1 class="text-4xl font-bold text-white mb-3 tracking-wide">OSCE</h1>
            <p class="text-xl text-gray-300">Objective Structured Clinical Examination Timer</p>
        </div>

        <!-- Timer Display -->
        <div class="glass-card rounded-3xl p-10 mb-8 text-center">
            <div class="timer-display mb-8" id="stopwatchDisplay">00:00:00</div>
            <div class="progress-bar">
                <div class="progress-fill" id="progressFill" style="width: 0%"></div>
            </div>
            <div class="text-lg text-gray-300 font-medium" id="statusText">Timer siap digunakan</div>
        </div>

        <!-- Buku Panduan Section -->
        <div class="glass-card rounded-3xl p-8 mb-8">
            <details class="group">
                <summary class="text-xl font-bold text-white mb-4 flex items-center gap-3 cursor-pointer">
                    <span class="w-2 h-2 bg-amber-500 rounded-full"></span>
                    Buku Panduan Penggunaan
                    <svg class="ml-auto w-5 h-5 text-gray-300 group-open:rotate-180 transition-transform" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7"></path>
                    </svg>
                </summary>
                <div class="text-gray-300 text-sm leading-relaxed space-y-4 mt-4">
                    <p>Selamat datang di Stopwatch OSCE! Aplikasi ini dirancang untuk membantu Anda mengatur waktu ujian OSCE dengan mudah dan efisien.</p>
                    
                    <h4 class="font-semibold text-white text-base">1. Pengaturan Timer Utama</h4>
                    <ul class="list-disc list-inside ml-4 space-y-1">
                        <li><strong>Menit & Detik:</strong> Masukkan durasi total timer yang Anda inginkan.</li>
                        <li><strong>Mulai Timer:</strong> Klik tombol ini untuk memulai hitung mundur.</li>
                        <li><strong>Reset:</strong> Menghentikan timer dan mengembalikannya ke 00:00:00.</li>
                    </ul>

                    <h4 class="font-semibold text-white text-base">2. Pengaturan Suara</h4>
                    <ul class="list-disc list-inside ml-4 space-y-1">
                        <li><strong>Suara AI:</strong> Pilih antara suara perempuan atau laki-laki untuk pesan suara. Klik "Test Suara" untuk mendengar contoh.</li>
                        <li><strong>Suara Bel:</strong> Pilih jenis suara bel yang akan berbunyi 5 detik sebelum pesan diucapkan dan saat waktu habis. Klik "Test Bel" untuk mendengar contoh.</li>
                    </ul>

                    <h4 class="font-semibold text-white text-base">3. Tambah Pesan Suara</h4>
                    <ul class="list-disc list-inside ml-4 space-y-1">
                        <li><strong>Pesan:</strong> Ketik pesan yang ingin diucapkan oleh AI pada waktu tertentu.</li>
                        <li><strong>Menit & Detik Pesan:</strong> Atur waktu (menit dan detik) kapan pesan ini akan diucapkan setelah timer dimulai.</li>
                        <li><strong>Simpan Pesan:</strong> Menambahkan pesan ke daftar.</li>
                        <li><strong>Test Pesan:</strong> Mendengar pesan yang sedang Anda ketik dengan suara AI yang dipilih.</li>
                    </ul>

                    <h4 class="font-semibold text-white text-base">4. Daftar Pesan Terjadwal</h4>
                    <ul class="list-disc list-inside ml-4 space-y-1">
                        <li>Daftar ini menampilkan semua pesan yang telah Anda tambahkan, diurutkan berdasarkan waktu.</li>
                        <li><strong>Status:</strong> Menunjukkan apakah pesan sedang menunggu, siap diucapkan (5 detik sebelum), atau sudah selesai diucapkan.</li>
                        <li><strong>Duplikat:</strong> Membuat salinan pesan dengan waktu yang sedikit berbeda.</li>
                        <li><strong>Edit:</strong> Membuka popup untuk mengedit pesan tanpa perlu scroll ke atas.</li>
                        <li><strong>Hapus:</strong> Menghapus pesan dari daftar.</li>
                    </ul>

                    <p class="mt-4">Semoga aplikasi ini bermanfaat untuk Anda!</p>
                </div>
            </details>
        </div>

        <div class="grid grid-cols-1 lg:grid-cols-2 gap-8">
            <!-- Timer Controls -->
            <div class="glass-card rounded-3xl p-8">
                <h3 class="text-xl font-bold text-white mb-6 flex items-center gap-3">
                    <span class="w-2 h-2 bg-blue-500 rounded-full"></span>
                    Pengaturan Timer
                </h3>
                <div class="grid grid-cols-2 gap-4 mb-6">
                    <div>
                        <label class="block text-sm font-semibold text-gray-300 mb-3">Menit</label>
                        <input id="minutesInput" type="number" min="0" max="60" value="0" class="input-field w-full">
                    </div>
                    <div>
                        <label class="block text-sm font-semibold text-gray-300 mb-3">Detik</label>
                        <input id="secondsInput" type="number" min="0" max="59" value="10" class="input-field w-full">
                    </div>
                </div>
                <div class="grid grid-cols-2 gap-4">
                    <button id="startTimerBtn" class="btn-primary w-full">
                        ▶️ Mulai Timer
                    </button>
                    <button id="resetTimerBtn" class="btn-secondary w-full">
                        ⏹️ Reset
                    </button>
                </div>
            </div>

            <!-- Voice & Bell Settings -->
            <div class="glass-card rounded-3xl p-8">
                <h3 class="text-xl font-bold text-white mb-6 flex items-center gap-3">
                    <span class="w-2 h-2 bg-purple-500 rounded-full"></span>
                    Pengaturan Suara
                </h3>
                <div class="space-y-6">
                    <div>
                        <label class="block text-sm font-semibold text-gray-300 mb-3">Suara AI</label>
                        <select id="voiceSelect" class="select-field w-full">
                            <!-- Options will be dynamically populated by JavaScript -->
                        </select>
                        <div class="voice-preview">
                            <button id="testVoiceBtn" type="button">🎤 Test Suara</button>
                            <span class="text-xs text-gray-400">Klik untuk mendengar contoh</span>
                        </div>
                    </div>
                    <div>
                        <label class="block text-sm font-semibold text-gray-300 mb-3">Suara Bel</label>
                        <select id="bellSelect" class="select-field w-full">
                            <option value="classic">🔔 Bel Klasik</option>
                            <option value="chime">🎵 Chime</option>
                            <option value="ding">🔊 Ding</option>
                            <option value="bell">🛎️ Bell</option>
                            <option value="notification">📢 Notifikasi</option>
                        </select>
                        <div class="bell-preview">
                            <button id="testBellBtn" type="button">🔔 Test Bel</button>
                            <span class="text-xs text-gray-400">Klik untuk mendengar contoh</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Message Form -->
        <div class="glass-card rounded-3xl p-8 mb-8 mt-8">
            <h3 class="text-xl font-bold text-white mb-6 flex items-center gap-3">
                <span class="w-2 h-2 bg-emerald-500 rounded-full"></span>
                Tambah Pesan Suara
            </h3>
            <div class="space-y-6">
                <div>
                    <label class="block text-sm font-semibold text-gray-300 mb-3">Pesan</label>
                    <textarea id="messageText" rows="3" placeholder="Masukkan pesan yang akan diucapkan..." class="input-field w-full resize-none"></textarea>
                </div>
                <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
                    <div>
                        <label class="block text-sm font-semibold text-gray-300 mb-3">Menit</label>
                        <input id="messageMinute" type="number" min="0" max="60" value="0" class="input-field w-full">
                    </div>
                    <div>
                        <label class="block text-sm font-semibold text-gray-300 mb-3">Detik</label>
                        <input id="messageSecond" type="number" min="0" max="59" value="10" class="input-field w-full">
                    </div>
                    <div class="flex items-end">
                        <button id="addMessageBtn" class="btn-success w-full">
                            💾 Simpan Pesan
                        </button>
                    </div>
                    <div class="flex items-end">
                        <button id="testMessageBtn" class="btn-primary w-full">
                            🎤 Test Pesan
                        </button>
                    </div>
                </div>
            </div>
        </div>

        <!-- Message List -->
        <div class="glass-card rounded-3xl p-8 mb-8">
            <h3 class="text-xl font-bold text-white mb-6 flex items-center gap-3">
                <span class="w-2 h-2 bg-cyan-500 rounded-full"></span>
                Daftar Pesan Terjadwal
            </h3>
            <div id="messageList">
                <div class="empty-state">
                    <div class="icon">📝</div>
                    <p class="text-xl font-semibold mb-2">Belum ada pesan</p>
                    <p class="text-sm">Tambahkan pesan untuk memulai</p>
                </div>
            </div>
        </div>

        <!-- Team Profile Section -->
        <div class="glass-card profile-section rounded-3xl p-8">
            <h3 class="text-xl font-bold text-white mb-6 flex items-center gap-3">
                <span class="w-2 h-2 bg-emerald-500 rounded-full"></span>
                Tim Pengembang OSCE Timer
            </h3>
            <p class="text-gray-300 text-sm mb-6 text-center">
                Kenali tim profesional yang mengembangkan aplikasi OSCE Timer ini dengan dedikasi tinggi
            </p>
            
            <div class="profile-grid">
                <!-- Profile 1 -->
                <a href="https://www.instagram.com/ivan.cava?utm_source=ig_web_button_share_sheet&igsh=ZDNlZDc0MzIxNw==" target="_blank" class="profile-card">
                    <div class="profile-link-icon">🔗</div>
                    <img src="profil7.jpg" alt="Ivan Cavanneva Royd Nastain" class="profile-image">
                    <h4 class="profile-name">Ivan Cavanneva Royd Nastain</h4>
                    <p class="profile-role">Frontend Developer & UI/UX Designer</p>
                    <p class="profile-description">Penggemar teknologi yang antusias mengeksplorasi perkembangan digital, aplikasi pintar, dan kecerdasan buatan. Menyukai membaca novel dari berbagai genre sebagai cara memahami emosi dan sudut pandang manusia. Juga menikmati film, baik fiksi maupun dokumenter, sebagai medium refleksi dan hiburan. Percaya bahwa teknologi, buku, dan film adalah kombinasi sempurna untuk memperluas wawasan dan membentuk imajinasi.</p>
                </a>

                <!-- Profile 2 -->
                <a href="https://www.instagram.com/nursandi_05?igsh=MXZmdWowaXM5enJrMQ==" target="_blank" class="profile-card">
                    <div class="profile-link-icon">🔗</div>
                    <img src="profil1.jpg" alt="Muhammad Nursandi" class="profile-image">
                    <h4 class="profile-name">Muhammad Nursandi</h4>
                    <p class="profile-role">Frontend Developer & UI/UX Designer</p>
                    <p class="profile-description">seorang mahasiswa jurusan program studi S1 Teknologi Informasi di Universitas Sari Mulia, memiliki minat mendalam pada inovasi digital. Fokus utamanya meliputi area transformatif seperti Internet of Things (IoT), Machine Learning, dan Kecerdasan Buatan (AI). Berpengalaman dalam merancang solusi teknologi melalui Program Kreativitas Mahasiswa Karsa Cipta (PKM-KC) dengan judul "Rancang Bangun Unnmanned Surface Vehicle Garbage Collector untuk meminimalisir sampah pada permukaan sungai berbasis IoT menggunakan Computer Vision", berdedikasi untuk memahami serta memanfaatkan potensi teknologi ini dalam menciptakan solusi nyata dan mendorong peluang baru.</p>
                </a>

                <!-- Profile 3 -->
                <a href="https://www.instagram.com/cavethestarve/?utm_source=ig_web_button_share_sheet" target="_blank" class="profile-card">
                    <div class="profile-link-icon">🔗</div>
                    <img src="profil3.jpg" alt="Akhmad Hafi Ilmiyanoor" class="profile-image">
                    <h4 class="profile-name">Akhmad Hafi Ilmiyanoor</h4>
                    <p class="profile-role">Frontend Developer & UI/UX Designer</p>
                    <p class="profile-description">seorang mahasiswa yang aktif UNISMmengembangkan berbagai proyek teknologi, terutama di bidang pengembangan web dan sistem informasi. Saya memiliki ketertarikan besar terhadap pembuatan sistem digital yang tidak hanya fungsional, tetapi juga interaktif dan menarik secara visual. Dalam perjalanan belajar , saya telah mengerjakan beragam proyek mulai dari website edukasi dan sistem penilaian berbasis COBIT 5, aplikasi pemilihan film dengan forum diskusi dan fitur rating. Dalam setiap proyek, saya selalu berusaha memadukan logika teknis dengan sentuhan desain yang engaging, terinspirasi dari gaya visual seperti Website Reverse 1999. Bagi saya, teknologi bukan hanya soal sistem yang berjalan baik, tapi juga soal bagaimana pengguna merasa nyaman, terhubung, dan tertarik untuk berinteraksi.</p>
                </a>

                <!-- Profile 4 -->
                <a href="https://www.instagram.com/exceldaudmasi?igsh=ZnA5MGJrYTlodmk5" target="_blank" class="profile-card">
                    <div class="profile-link-icon">🔗</div>
                    <img src="profil2.jpg" alt="Excel Daud" class="profile-image">
                    <h4 class="profile-name">Excel Daud</h4>
                    <p class="profile-role">Frontend Developer & UI/UX Designer</p>
                    <p class="profile-description">Saya aktif mengeksplorasi berbagai bahasa pemrograman dan platform pengembangan, serta mengikuti perkembangan terbaru di dunia AI seperti machine learning, natural language processing, dan computer vision. Saya percaya bahwa kombinasi antara logika pemrograman dan kecerdasan buatan akan menjadi fondasi penting dalam menciptakan inovasi digital di masa depan.</p>
                </a>

                <!-- Profile 5 -->
                <a href="https://www.instagram.com/sultnnr_?utm_source=ig_web_button_share_sheet&igsh=ZDNlZDc0MzIxNw==" target="_blank" class="profile-card">
                    <div class="profile-link-icon">🔗</div>
                    <img src="profil6.jpg" alt="Sultan Nur Rahman" class="profile-image">
                    <h4 class="profile-name">Sultan Nur Rahman</h4>
                    <p class="profile-role">Frontend Developer & UI/UX Designer</p>
                    <p class="profile-description">Saya Memiliki ketertarikan di bidang Digital Creative dan Photography. Sebagai seseorang yang memiliki minat di bidang tersebut, saya memiliki passion di bidang editing foto dan design visual. Saya memiliki keahlian dan ketertarikan pada Kamera.</p>
                </a>

                <!-- Profile 6 -->
                <a href="https://www.instagram.com/wvnx___/?utm_source=ig_web_button_share_sheet" target="_blank" class="profile-card">
                    <div class="profile-link-icon">🔗</div>
                    <img src="profil4.jpg" alt="Daniel Marvelino Septian" class="profile-image">
                    <h4 class="profile-name">Daniel Marvelino Septian</h4>
                    <p class="profile-role">Frontend Developer & UI/UX Designer</p>
                    <p class="profile-description">Saya, Daniel Marvelino Septian, adalah mahasiswa Aktif Program Studi Sarjana Teknologi Informasi di Universitas Sari Mulia memiliki passion yang kuat dalam bidang Software Engineering dan Kecerdasan Buatan (AI). Saya berkomitmen untuk terus mengasah keterampilan dan pengetahuan saya dalam pengembangan perangkat lunak dan desain antarmuka, didorong oleh motivasi tinggi untuk terus belajar dan berkembang di dunia teknologi yang dinamis.</p>
                </a>

                <!-- Profile 7 -->
                <a href="https://www.instagram.com/mikhael_ny?utm_source=ig_web_button_share_sheet&igsh=ZDNlZDc0MzIxNw==" target="_blank" class="profile-card">
                    <div class="profile-link-icon">🔗</div>
                    <img src="profil5.jpg" alt="Mikhael Neta Yahu" class="profile-image">
                    <h4 class="profile-name">Mikhael Neta Yahu</h4>
                    <p class="profile-role">Frontend Developer & UI/UX Designer</p>
                    <p class="profile-description">Saya adalah mahasiswa Program Studi S1 Teknologi Informasi di Universitas Sari Mulia yang memiliki minat besar dalam bidang Artificial Intelligence (AI) dan pemrograman. Ketertarikan saya terhadap teknologi mendorong saya untuk terus belajar dan mengembangkan kemampuan dalam coding, khususnya dalam membangun solusi cerdas yang dapat membantu memecahkan berbagai permasalahan nyata.</p>
                </a>
            </div>
        </div>
    </div>

    <!-- Audio elements -->
    <audio id="notifSound" preload="auto"></audio>

    <script>
        // Tutorial Variables
        let currentSlideIndex = 0;
        const totalSlides = 15;

        // App Variables
        let timerInterval = null;
        let elapsedSeconds = 0;
        let messages = [];
        let editIndex = -1;
        let targetSeconds = 0;
        let isRunning = false;
        let selectedVoice = '';
        let selectedBell = 'classic';
        let continuousBellInterval = null;

        // DOM elements
        const tutorialOverlay = document.getElementById("tutorialOverlay");
        const sliderTrack = document.getElementById("sliderTrack");
        const currentSlideSpan = document.getElementById("currentSlide");
        const totalSlidesSpan = document.getElementById("totalSlides");
        const prevBtn = document.getElementById("prevBtn");
        const nextBtn = document.getElementById("nextBtn");
        const sliderDots = document.getElementById("sliderDots");
        const tutorialStartBtn = document.getElementById("startBtn");

        const display = document.getElementById("stopwatchDisplay");
        const progressFill = document.getElementById("progressFill");
        const statusText = document.getElementById("statusText");
        const minutesInput = document.getElementById("minutesInput");
        const secondsInput = document.getElementById("secondsInput");
        const startBtn = document.getElementById("startTimerBtn");
        const resetBtn = document.getElementById("resetTimerBtn");
        const messageText = document.getElementById("messageText");
        const messageMinute = document.getElementById("messageMinute");
        const messageSecond = document.getElementById("messageSecond");
        const addMessageBtn = document.getElementById("addMessageBtn");
        const testMessageBtn = document.getElementById("testMessageBtn");
        const messageList = document.getElementById("messageList");
        const voiceSelect = document.getElementById("voiceSelect");
        const bellSelect = document.getElementById("bellSelect");
        const testVoiceBtn = document.getElementById("testVoiceBtn");
        const testBellBtn = document.getElementById("testBellBtn");

        // Modal elements
        const editModal = document.getElementById("editModal");
        const editMessageText = document.getElementById("editMessageText");
        const editMessageMinute = document.getElementById("editMessageMinute");
        const editMessageSecond = document.getElementById("editMessageSecond");
        const updateMessageBtn = document.getElementById("updateMessageBtn");
        const testEditMessageBtn = document.getElementById("testEditMessageBtn");

        // Tutorial Functions
        function initializeTutorial() {
            totalSlidesSpan.textContent = totalSlides;
            createDots();
            updateSlider();
        }

        function createDots() {
            sliderDots.innerHTML = '';
            for (let i = 0; i < totalSlides; i++) {
                const dot = document.createElement('div');
                dot.className = `dot ${i === 0 ? 'active' : ''}`;
                dot.onclick = () => goToSlide(i);
                sliderDots.appendChild(dot);
            }
        }

        function updateSlider() {
            const translateX = -currentSlideIndex * 100;
            sliderTrack.style.transform = `translateX(${translateX}%)`;
            currentSlideSpan.textContent = currentSlideIndex + 1;

            // Update dots
            const dots = sliderDots.querySelectorAll('.dot');
            dots.forEach((dot, index) => {
                dot.classList.toggle('active', index === currentSlideIndex);
            });

            // Update navigation buttons
            prevBtn.classList.toggle('disabled', currentSlideIndex === 0);
            nextBtn.classList.toggle('disabled', currentSlideIndex === totalSlides - 1);

            // Show start button on last slide
            if (currentSlideIndex === totalSlides - 1) {
                tutorialStartBtn.style.display = 'inline-block';
            } else {
                tutorialStartBtn.style.display = 'none';
            }
        }

        function nextSlide() {
            if (currentSlideIndex < totalSlides - 1) {
                currentSlideIndex++;
                updateSlider();
            }
        }

        function previousSlide() {
            if (currentSlideIndex > 0) {
                currentSlideIndex--;
                updateSlider();
            }
        }

        function goToSlide(index) {
            currentSlideIndex = index;
            updateSlider();
        }

        function skipTutorial() {
            startApp();
        }

        function startApp() {
            tutorialOverlay.classList.add('hidden');
            setTimeout(() => {
                tutorialOverlay.style.display = 'none';
            }, 500);
        }

        // Initialize floating particles
        function createParticles() {
            const particlesContainer = document.getElementById('particles');
            const particleCount = 20;

            for (let i = 0; i < particleCount; i++) {
                const particle = document.createElement('div');
                particle.className = 'particle';
                particle.style.left = Math.random() * 100 + '%';
                particle.style.animationDelay = Math.random() * 20 + 's';
                particle.style.animationDuration = (Math.random() * 10 + 15) + 's';
                particlesContainer.appendChild(particle);
            }
        }

        // Utility functions
        function formatTime(seconds) {
            const h = Math.floor(seconds / 3600).toString().padStart(2, "0");
            const m = Math.floor((seconds % 3600) / 60).toString().padStart(2, "0");
            const s = (seconds % 60).toString().padStart(2, "0");
            return `${h}:${m}:${s}`;
        }

        function createBellSound(type) {
            try {
                const audioContext = new (window.AudioContext || window.webkitAudioContext)();
                const oscillator = audioContext.createOscillator();
                const gainNode = audioContext.createGain();

                oscillator.connect(gainNode);
                gainNode.connect(audioContext.destination);

                let frequency = 800;
                let duration = 0.5;

                switch(type) {
                    case 'classic':
                        frequency = 800;
                        oscillator.type = 'sine';
                        break;
                    case 'chime':
                        frequency = 1000;
                        oscillator.type = 'triangle';
                        duration = 1.0;
                        break;
                    case 'ding':
                        frequency = 1200;
                        oscillator.type = 'square';
                        duration = 0.3;
                        break;
                    case 'bell':
                        frequency = 880;
                        oscillator.type = 'sine';
                        duration = 0.8;
                        break;
                    case 'notification':
                        frequency = 600;
                        oscillator.type = 'sawtooth';
                        duration = 0.4;
                        break;
                }

                oscillator.frequency.value = frequency;
                gainNode.gain.setValueAtTime(0.3, audioContext.currentTime);
                gainNode.gain.exponentialRampToValueAtTime(0.01, audioContext.currentTime + duration);

                oscillator.start(audioContext.currentTime);
                oscillator.stop(audioContext.currentTime + duration);

                // Add a second tone for chime effect
                if (type === 'chime') {
                    const oscillator2 = audioContext.createOscillator();
                    const gainNode2 = audioContext.createGain();
                    oscillator2.connect(gainNode2);
                    gainNode2.connect(audioContext.destination);
                    oscillator2.frequency.value = frequency * 1.5;
                    oscillator2.type = 'triangle';
                    gainNode2.gain.setValueAtTime(0.2, audioContext.currentTime + 0.1);
                    gainNode2.gain.exponentialRampToValueAtTime(0.01, audioContext.currentTime + duration);
                    oscillator2.start(audioContext.currentTime + 0.1);
                    oscillator2.stop(audioContext.currentTime + duration);
                }
            } catch (e) {
                console.log('Audio context not supported');
            }
        }

        // Function to start continuous bell sound
        function startContinuousBell(type, durationMs, intervalMs) {
            stopContinuousBell(); // Ensure any previous continuous bell is stopped
            const startTime = Date.now();
            continuousBellInterval = setInterval(() => {
                if (Date.now() - startTime < durationMs) {
                    createBellSound(type);
                } else {
                    stopContinuousBell(); // Stop when duration is reached
                }
            }, intervalMs);
        }

        // Function to stop continuous bell sound
        function stopContinuousBell() {
            if (continuousBellInterval) {
                clearInterval(continuousBellInterval);
                continuousBellInterval = null;
            }
        }

        // Modified speakText function to handle dynamic voices
        function speakText(text, voiceName) {
            return new Promise((resolve) => {
                const utterance = new SpeechSynthesisUtterance(text);
                utterance.lang = "id-ID"; // Prioritize Indonesian language
                utterance.rate = 0.85;
                utterance.volume = 0.8;

                const voices = speechSynthesis.getVoices();
                let targetVoice = null;

                // 1. Try to find the exact voice by name
                targetVoice = voices.find(v => v.name === voiceName);

                // 2. If not found, try to find an Indonesian voice
                if (!targetVoice) {
                    const indonesianVoices = voices.filter(v => v.lang.includes('id') || v.lang.includes('ID'));
                    if (indonesianVoices.length > 0) {
                        // Try to find a gender-matching Indonesian voice if voiceName implies gender
                        const lowerVoiceName = voiceName.toLowerCase();
                        if (lowerVoiceName.includes('female') || lowerVoiceName.includes('perempuan')) {
                            targetVoice = indonesianVoices.find(v => 
                                v.name.toLowerCase().includes('female') || 
                                v.name.toLowerCase().includes('perempuan')
                            ) || indonesianVoices[0];
                        } else if (lowerVoiceName.includes('male') || lowerVoiceName.includes('laki-laki')) {
                            targetVoice = indonesianVoices.find(v => 
                                v.name.toLowerCase().includes('male') || 
                                v.name.toLowerCase().includes('laki-laki')
                            ) || indonesianVoices[0];
                        } else {
                            targetVoice = indonesianVoices[0]; // Default to first Indonesian voice
                        }
                    }
                }

                // 3. Fallback to general gender-based selection if no specific voice or Indonesian voice found
                if (!targetVoice) {
                    const genderVoices = voices.filter(v => {
                        const name = v.name.toLowerCase();
                        return voiceName.toLowerCase().includes('female') ? 
                            (name.includes('female') || name.includes('woman') || name.includes('zira') || name.includes('hazel')) :
                            (name.includes('male') || name.includes('man') || name.includes('david') || name.includes('mark'));
                    });
                    if (genderVoices.length > 0) {
                        targetVoice = genderVoices[0];
                    }
                }

                // 4. If a voice is found, set it and adjust pitch
                if (targetVoice) {
                    utterance.voice = targetVoice;
                    // Adjust pitch based on selected voice's gender if known, otherwise default
                    const voiceGender = targetVoice.name.toLowerCase().includes('female') ? 'female' : 
                                       (targetVoice.name.toLowerCase().includes('male') ? 'male' : null);
                    utterance.pitch = voiceGender === 'female' ? 1.2 : (voiceGender === 'male' ? 0.8 : 1); // Default pitch if gender unknown
                } else {
                    // Fallback pitch if no specific voice could be set
                    utterance.pitch = voiceName.toLowerCase().includes('female') ? 1.2 : 0.8;
                }

                utterance.onend = () => resolve();
                utterance.onerror = () => resolve();
                speechSynthesis.speak(utterance);
            });
        }

        // New function to populate voice list
        function populateVoiceList() {
            const voices = speechSynthesis.getVoices();
            voiceSelect.innerHTML = ''; // Clear existing options

            // Filter for Indonesian voices first
            const indonesianVoices = voices.filter(voice => voice.lang.includes('id') || voice.lang.includes('ID'));

            if (indonesianVoices.length > 0) {
                // Add Indonesian voices
                indonesianVoices.forEach(voice => {
                    const option = document.createElement('option');
                    option.textContent = `${voice.name} (${voice.lang})`;
                    option.value = voice.name; // Use voice.name as the value
                    if (voice.default) {
                        option.selected = true;
                        selectedVoice = voice.name; // Set default selected voice
                    }
                    voiceSelect.appendChild(option);
                });
            } else {
                // Fallback if no Indonesian voices are found
                const defaultOption = document.createElement('option');
                defaultOption.textContent = "Tidak ada suara Indonesia ditemukan. Menggunakan suara default browser.";
                defaultOption.value = "default";
                voiceSelect.appendChild(defaultOption);

                // Add some common English voices as fallback if no ID voices
                voices.filter(v => v.lang.startsWith('en')).slice(0, 5).forEach(voice => {
                    const option = document.createElement('option');
                    option.textContent = `${voice.name} (${voice.lang})`;
                    option.value = voice.name;
                    voiceSelect.appendChild(option);
                });
            }

            // Set the initial selectedVoice based on the dropdown if not already set
            if (!selectedVoice && voiceSelect.options.length > 0) {
                selectedVoice = voiceSelect.value;
            }
        }

        function showNotification(message, type = 'info') {
            const notification = document.createElement('div');
            notification.className = `notification ${type}`;
            notification.textContent = message;
            document.body.appendChild(notification);

            setTimeout(() => {
                notification.style.opacity = '0';
                notification.style.transform = 'translateX(100%)';
                setTimeout(() => notification.remove(), 300);
            }, 3000);
        }

        function updateDisplay() {
            display.textContent = formatTime(elapsedSeconds);

            if (isRunning) {
                display.classList.add('timer-active');
                if (targetSeconds > 0) {
                    const progress = (elapsedSeconds / targetSeconds) * 100;
                    progressFill.style.width = Math.min(progress, 100) + '%';
                    const remaining = targetSeconds - elapsedSeconds;
                    statusText.textContent = remaining > 0 ? `Sisa waktu: ${formatTime(remaining)}` : 'Waktu habis!';
                } else {
                    statusText.textContent = 'Timer berjalan...';
                }
            } else {
                display.classList.remove('timer-active');
                statusText.textContent = 'Timer siap digunakan';
            }
        }

        function renderMessages() {
            if (messages.length === 0) {
                messageList.innerHTML = `
                    <div class="empty-state">
                        <div class="icon">📝</div>
                        <p class="text-xl font-semibold mb-2">Belum ada pesan</p>
                        <p class="text-sm">Tambahkan pesan untuk memulai</p>
                    </div>
                `;
                return;
            }

            messageList.innerHTML = '';
            messages.forEach((msg, index) => {
                const div = document.createElement('div');
                const timeText = formatTime(msg.time);
                let status = 'pending';
                let statusIcon = '⏰';
                let statusLabel = 'Menunggu';

                if (isRunning) {
                    if (elapsedSeconds >= msg.time - 5 && elapsedSeconds < msg.time) {
                        status = 'active';
                        statusIcon = '🔔';
                        statusLabel = 'Siap';
                    } else if (elapsedSeconds >= msg.time) {
                        status = 'completed';
                        statusIcon = '✅';
                        statusLabel = 'Selesai';
                    }
                }

                div.className = `message-item slide-in ${status === 'active' ? 'active' : ''}`;
                div.innerHTML = `
                    <div class="flex justify-between items-start gap-4">
                        <div class="flex-1">
                            <div class="flex items-center gap-3 mb-3">
                                <span class="status-badge ${status}">
                                    ${statusIcon} ${timeText}
                                </span>
                                <span class="text-xs text-gray-400 font-medium">${statusLabel}</span>
                            </div>
                            <p class="text-gray-200 leading-relaxed text-sm">${msg.text}</p>
                        </div>
                        <div class="flex flex-col gap-2">
                            <div class="flex gap-2">
                                <button onclick="duplicateMessage(${index})" class="btn-duplicate">
                                    📋 Duplikat
                                </button>
                                <button onclick="editMessage(${index})" class="btn-edit">
                                    ✏️ Edit
                                </button>
                            </div>
                            <button onclick="deleteMessage(${index})" class="btn-danger w-full">
                                🗑️ Hapus
                            </button>
                        </div>
                    </div>
                `;
                messageList.appendChild(div);
            });
        }

        function addOrEditMessage() {
            const text = messageText.value.trim();
            const min = parseInt(messageMinute.value, 10) || 0;
            const sec = parseInt(messageSecond.value, 10) || 0;
            const totalSec = min * 60 + sec;

            if (!text) {
                showNotification("Pesan tidak boleh kosong!", "error");
                return;
            }

            if (totalSec < 0) {
                showNotification("Waktu tidak valid!", "error");
                return;
            }

            messages.push({ text, time: totalSec, spoken: false, notified: false });
            showNotification("Pesan berhasil ditambahkan!", "success");

            messageText.value = "";
            messageMinute.value = 0;
            messageSecond.value = 0;

            messages.sort((a, b) => a.time - b.time);
            renderMessages();
        }

        // Modal functions
        function openEditModal(index) {
            const msg = messages[index];
            editMessageText.value = msg.text;
            editMessageMinute.value = Math.floor(msg.time / 60);
            editMessageSecond.value = msg.time % 60;
            editIndex = index;
            editModal.classList.add('active');
            editMessageText.focus();
        }

        function closeEditModal() {
            editModal.classList.remove('active');
            editIndex = -1;
            editMessageText.value = "";
            editMessageMinute.value = 0;
            editMessageSecond.value = 0;
        }

        function updateMessage() {
            const text = editMessageText.value.trim();
            const min = parseInt(editMessageMinute.value, 10) || 0;
            const sec = parseInt(editMessageSecond.value, 10) || 0;
            const totalSec = min * 60 + sec;

            if (!text) {
                showNotification("Pesan tidak boleh kosong!", "error");
                return;
            }

            if (totalSec < 0) {
                showNotification("Waktu tidak valid!", "error");
                return;
            }

            if (editIndex !== -1) {
                messages[editIndex] = { text, time: totalSec, spoken: false, notified: false };
                messages.sort((a, b) => a.time - b.time);
                renderMessages();
                closeEditModal();
                showNotification("Pesan berhasil diperbarui!", "success");
            }
        }

        function testEditMessage() {
            const text = editMessageText.value.trim();
            if (!text) {
                showNotification("Masukkan pesan terlebih dahulu!", "error");
                return;
            }
            speakText(text, selectedVoice);
        }

        function editMessage(index) {
            openEditModal(index);
        }

        function duplicateMessage(index) {
            const msg = messages[index];
            const duplicatedMsg = {
                text: msg.text + " (Duplikat)",
                time: msg.time + 30, // Add 30 seconds to avoid conflict
                spoken: false,
                notified: false
            };
            messages.push(duplicatedMsg);
            messages.sort((a, b) => a.time - b.time);
            renderMessages();
            showNotification("Pesan berhasil diduplikat!", "success");
        }

        function deleteMessage(index) {
            if (confirm("Yakin ingin menghapus pesan ini?")) {
                messages.splice(index, 1);
                renderMessages();
                showNotification("Pesan berhasil dihapus!", "info");
            }
        }

        function startTimer() {
            if (timerInterval) return;

            const mins = parseInt(minutesInput.value, 10) || 0;
            const secs = parseInt(secondsInput.value, 10) || 0;

            if (mins === 0 && secs === 0) {
                showNotification("Masukkan waktu yang valid!", "error");
                return;
            }

            targetSeconds = mins * 60 + secs;
            elapsedSeconds = 0;
            isRunning = true;
            progressFill.style.width = '0%';

            messages.forEach(msg => {
                msg.spoken = false;
                msg.notified = false;
            });

            startBtn.innerHTML = '⏸️ Timer Berjalan...';
            startBtn.disabled = true;
            showNotification("Timer dimulai!", "success");

            timerInterval = setInterval(() => {
                elapsedSeconds++;
                updateDisplay();
                renderMessages();

                messages.forEach(msg => {
                    if (!msg.notified && elapsedSeconds === msg.time - 5) {
                        // Start continuous bell sound for 5 seconds
                        startContinuousBell(selectedBell, 5000, 200); // Play for 5 seconds, every 200ms
                        msg.notified = true;
                        showNotification(`5 detik lagi: ${msg.text}`, "info");
                    }

                    if (!msg.spoken && elapsedSeconds === msg.time) {
                        stopContinuousBell(); // Stop the bell when the message is spoken
                        speakText(msg.text, selectedVoice);
                        msg.spoken = true;
                        showNotification(`Pesan diucapkan: ${msg.text}`, "success");
                    }
                });

                if (targetSeconds > 0 && elapsedSeconds >= targetSeconds) {
                    resetTimer();
                    showNotification("Waktu habis!", "info");
                    createBellSound(selectedBell); // Play bell once when time is up
                }
            }, 1000);
        }

        function resetTimer() {
            clearInterval(timerInterval);
            timerInterval = null;
            elapsedSeconds = 0;
            isRunning = false;
            progressFill.style.width = '0%';
            stopContinuousBell(); // Stop any ongoing bell sound on reset

            messages.forEach(msg => {
                msg.spoken = false;
                msg.notified = false;
            });

            startBtn.innerHTML = '▶️ Mulai Timer';
            startBtn.disabled = false;
            updateDisplay();
            renderMessages();
            showNotification("Timer direset!", "info");
        }

        function testVoice() {
            const testText = "Halo, ini contoh suara AI yang dipilih.";
            speakText(testText, selectedVoice);
        }

        function testBell() {
            // Test bell by playing it a few times with a short delay
            createBellSound(selectedBell);
            setTimeout(() => createBellSound(selectedBell), 150);
            setTimeout(() => createBellSound(selectedBell), 300);
        }

        function testMessage() {
            const text = messageText.value.trim();
            if (!text) {
                showNotification("Masukkan pesan terlebih dahulu!", "error");
                return;
            }
            speakText(text, selectedVoice);
        }

        // Event listeners
        startBtn.addEventListener("click", startTimer);
        resetBtn.addEventListener("click", resetTimer);
        addMessageBtn.addEventListener("click", addOrEditMessage);
        testMessageBtn.addEventListener("click", testMessage);
        testVoiceBtn.addEventListener("click", testVoice);
        testBellBtn.addEventListener("click", testBell);
        updateMessageBtn.addEventListener("click", updateMessage);
        testEditMessageBtn.addEventListener("click", testEditMessage);

        voiceSelect.addEventListener("change", (e) => {
            selectedVoice = e.target.value; // Now stores the voice name
        });

        bellSelect.addEventListener("change", (e) => {
            selectedBell = e.target.value;
        });

        messageText.addEventListener("keypress", (e) => {
            if (e.key === "Enter" && !e.shiftKey) {
                e.preventDefault();
                addOrEditMessage();
            }
        });

        // Close modal when clicking outside
        editModal.addEventListener("click", (e) => {
            if (e.target === editModal) {
                closeEditModal();
            }
        });

        // Close modal with Escape key
        document.addEventListener("keydown", (e) => {
            if (e.key === "Escape" && editModal.classList.contains('active')) {
                closeEditModal();
            }
        });

        // Keyboard navigation for tutorial
        document.addEventListener("keydown", (e) => {
            if (!tutorialOverlay.classList.contains('hidden')) {
                if (e.key === "ArrowLeft") {
                    previousSlide();
                } else if (e.key === "ArrowRight") {
                    nextSlide();
                } else if (e.key === "Escape") {
                    skipTutorial();
                }
            }
        });

        // Initialize
        initializeTutorial();
        createParticles();
        updateDisplay();
        renderMessages();
        populateVoiceList();

        // Load voices when available (important for some browsers)
        if (speechSynthesis.onvoiceschanged !== undefined) {
            speechSynthesis.onvoiceschanged = function() {
                populateVoiceList(); // Call when voices change
            };
        }

        // Global functions
        window.editMessage = editMessage;
        window.deleteMessage = deleteMessage;
        window.duplicateMessage = duplicateMessage;
        window.closeEditModal = closeEditModal;
        window.nextSlide = nextSlide;
        window.previousSlide = previousSlide;
        window.skipTutorial = skipTutorial;
        window.startApp = startApp;
    </script>
</body>
</html>
