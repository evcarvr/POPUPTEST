/* Reset and base styles */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Segoe UI', sans-serif;
}

body, html {
  height: 100%;
  background: #f4f4f4;
  display: flex;
  flex-direction: column;
  overflow: hidden; /* Prevent scrollbars caused by fixed elements */
}

/* Map container fills available space */
#map {
  flex-grow: 1;
  height: 100%;
  z-index: 1;
}
#appHeader {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 60px;
  background: linear-gradient(90deg, #0d47a1, #1976d2, #42a5f5);
  color: white;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  font-weight: 900;
  font-size: 1.5rem;
  /* Center horizontally and vertically */
  display: flex;
  align-items: center;        /* <-- This makes icon & text line up on their centers */
  justify-content: center;    /* Centers the combo in the header */
  text-align: left;           /* Prevents centering inside header if not desired */
  z-index: 10000;
  user-select: none;
  box-shadow: 0 2px 6px rgba(0,0,0,0.15);
  box-sizing: border-box;
  padding: 0;
}

#appLogoIcon {
  height: 28px;
  width: 28px;
  margin-right: 12px;
  border-radius: 8px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.09);
  background: white;
  display: inline-block;
  /* No vertical-align needed thanks to flex */
}


/* Shift the #controls-top down below header */
#controls-top {
  position: fixed;
  top: 60px; /* Same height as #appHeader */
  left: 0;
  width: 100%;
  background: white;
  /* keep your existing styles, just add margin top */
  box-shadow: 0 2px 4px rgba(0,0,0,0.2);
  padding: 10px;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  align-items: center;
  gap: 10px;
  z-index: 9999;
}


/* Buttons inside top controls */
#controls-top button {
  padding: 10px 14px;
  border: none;
  border-radius: 25px;
  font-size: 15px;
  font-weight: 600;
  cursor: pointer;
  transition: background-color 0.3s ease;
  color: white;
  user-select: none;
}

/* Specific buttons with colors and hover */
#clearBtn {
  background: #e74c3c;
}
#clearBtn:hover {
  background: #c0392b;
}

#saveBtn {
  background: #2980b9;
}
#saveBtn:hover {
  background: #2471a3;
}

#loadBtn {
  background: #27ae60;
}
#loadBtn:hover {
  background: #1e8449;
}

#shareBtn {
  background: #f39c12;
}
#shareBtn:hover {
  background: #d68910;
}

/* Share link input box */
#shareLink {
  flex-grow: 1;
  min-width: 200px;
  padding: 10px;
  border-radius: 25px;
  border: 1px solid #ccc;
  font-size: 14px;
  cursor: pointer;
  user-select: all;
  color: #333;
}

/* Bottom controls container */
.controls-bottom {
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
  background: white;
  padding: 15px;
  box-shadow: 0 -2px 6px rgba(0,0,0,0.1);
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 10px;
  z-index: 10000;
}

/* Progress bar wrapper */
#progressBarWrapper {
  width: 80%;
  max-width: 600px;
  text-align: center;
  display: none; /* shown dynamically */
}

/* Progress text above bar */
#progressText {
  font-weight: 600;
  margin-bottom: 6px;
  color: #333;
}

/* Outer bar */
#progressOuter {
  background: #ddd;
  height: 12px;
  border-radius: 10px;
  overflow: hidden;
  margin-bottom: 6px;
}

/* Inner progress bar */
#progressInner {
  height: 100%;
  width: 0;
  background: linear-gradient(90deg, #007bff, #00c6ff);
  transition: width 0.3s ease;
}

/* ETA text */
#etaText {
  color: #666;
  font-size: 14px;
}

/* Start Navigation button */
#startNavBtn {
  background: linear-gradient(135deg, #007bff, #00c6ff);
  color: white;
  font-size: 18px;
  padding: 15px 40px;
  border-radius: 30px;
  border: none;
  cursor: pointer;
  box-shadow: 0 4px 8px rgba(0,0,0,0.2);
  font-weight: 600;
  transition: background 0.3s ease;
  animation: pulse 1.5s infinite;
  user-select: none;
}

#startNavBtn:hover:not(:disabled) {
  background: linear-gradient(135deg, #0056b3, #0099cc);
}

#startNavBtn:disabled {
  background: #a3c8ff;
  cursor: not-allowed;
  animation: none; /* stop pulse animation */
}

/* Button pulse animation */
@keyframes pulse {
  0% { transform: scale(1); }
  50% { transform: scale(1.03); }
  100% { transform: scale(1); }
}

/* Responsive layout changes */
@media (max-width: 768px) {
  #controls-top {
    justify-content: center;
  }
  #controls-top button {
    flex: 1 1 40%;
  }
}

@media (max-width: 480px) {
  #startNavBtn {
    width: 90%;
    font-size: 16px;
  }
}

/* Popup overlay - semi-transparent dark background covering entire viewport */
.popup-overlay {
  position: fixed;
  top: 0; left: 0; right: 0; bottom: 0;
  background: rgba(0,0,0,0.5);
  display: none; /* hidden until shown by JS */
  justify-content: center;
  align-items: center;
  z-index: 20000;
}

/* Popup container */
.popup {
  background: white;
  width: 90%;
  max-width: 400px;
  border-radius: 12px;
  box-shadow: 0 20px 50px rgba(0,0,0,0.15);
  padding: 30px 25px;
  text-align: center;
  position: relative;
  animation: slideIn 0.3s ease forwards;
  user-select: none;
}

/* Popup title */
.popup h2,
.alert-title {
  margin-bottom: 20px;
  color: #333;
  font-weight: bold;
  font-size: 1.8rem;
}

/* Alert description paragraph */
.popup p,
.alert-desc {
  color: #555;
  font-size: 1.1rem;
  margin-bottom: 30px;
  font-weight: 500;
}

/* Close button (the X) */
.btn-close-popup {
  position: absolute;
  top: 15px;
  right: 15px;
  background: transparent;
  border: none;
  font-size: 24px;
  cursor: pointer;
  color: #aaa;
  transition: color 0.2s ease;
}
.btn-close-popup:hover {
  color: #007bff;
}

/* "Awesome!" completion button */
#awesomeBtn {
  margin-top: 10px;
  background: #16c60c;
  color: white;
  font-size: 1.1rem;
  font-weight: bold;
  border: none;
  border-radius: 8px;
  padding: 12px 32px;
  cursor: pointer;
  box-shadow: 0 4px 16px rgba(22,198,12,0.18);
  transition: background 0.2s, transform 0.17s;
  user-select: none;
}
#awesomeBtn:hover {
  background: #05990b;
  transform: scale(1.04);
}

/* "Got it" button on route deviation alert */
#gotItAlertBtn {
  margin-top: 10px;
  background: #e74c3c;
  color: white;
  font-size: 1.1rem;
  font-weight: bold;
  border: none;
  border-radius: 8px;
  padding: 12px 32px;
  cursor: pointer;
  box-shadow: 0 4px 16px rgba(231,76,60,0.18);
  transition: background 0.2s, transform 0.17s;
  user-select: none;
}
#gotItAlertBtn:hover {
  background: #b82414;
  transform: scale(1.04);
}

/* Popup show animation */
@keyframes slideIn {
  from {
    opacity: 0;
    transform: translateY(-20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
