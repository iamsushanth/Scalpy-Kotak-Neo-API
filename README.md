# Scalpy-Kotak-Neo-API
Scalpy App is a professional-grade desktop trading utility application for options trading on Indian markets through Kotak Neo API. Built with Python and Tkinter, it provides advanced order management, automated stop-loss/target placement, real-time market data, and intelligent trailing stop-loss functionality.

## 🎯 Core Features

### 📊 **Real-Time Market Data**
- Live price feeds for NIFTY, BANKNIFTY, SENSEX, BANKEX
- Real-time LTP (Last Traded Price) updates
- WebSocket-based streaming for zero-latency data
- Multi-symbol concurrent subscriptions

### 🔧 **Advanced Order Management**
- **Order Types**: Market (MKT), Limit (LMT), Stop-Loss Limit (SL-LMT)
- **Product Types**: MIS (Intraday), NRML (Normal), BO (Bracket Order), CO (Cover Order)
- **Both Sides Trading**:
  - **BUY Orders** - Long positions (Call/Put options)
  - **SELL Orders** - Short positions (Call/Put options)
- **Strike Selection**: ATM, ITM1-4, OTM1-20 for precise positioning
- **Multi-Index Support**: NIFTY, BANKNIFTY, FINNIFTY, MIDCPNIFTY, SENSEX, BANKEX

### 🛡️ **Intelligent Risk Management**

#### **Automatic SL/Target Placement**
When an order is executed, Scalpy Pro automatically places:
- **For BUY Positions**: 
  - Stop-Loss BELOW entry price (SELL order)
  - Target ABOVE entry price (SELL order)
- **For SELL Positions**:
  - Stop-Loss ABOVE entry price (BUY order)
  - Target BELOW entry price (BUY order)

#### **Dynamic Trailing Stop-Loss**
- **Buy-Side Trailing**: SL trails UPWARD as price increases
- **Sell-Side Trailing**: SL trails DOWNWARD as price decreases
- **Target-Based Activation**: Automatic trailing after profit milestones
- **Smart Updates**: Only moves SL in favorable direction (never worsens)
- **Validation**: Checks before every update to prevent degradation

### 🚀 **One-Click Trading**
- **Quick Entry Buttons**:
  - `Buy CE` - Buy CALL options (bullish)
  - `Buy PE` - Buy PUT options (bearish)
  - `Sell CE` - Sell CALL options (bearish/premium collection)
  - `Sell PE` - Sell PUT options (bullish/premium collection)
- **Instant Execution**: Market orders execute within milliseconds
- **Visual Feedback**: Color-coded buttons and status messages

### 📊 **Position Management**
- **Real-Time P&L Tracking**: MTM (Mark-to-Market) updates
- **Net Quantity Calculation**: Accurate position sizing
- **Position Book**: Complete view of all open positions
- **Universal Exit**: One-click square-off of all positions
- **Selective Exit**: Close specific CE or PE positions

### 🔄 **Smart Automation**

#### **Auto-Trail Mode**
- Continuously monitors positions
- Automatically adjusts stop-losses based on market movement
- Configurable trailing buffer
- Works for both long and short positions

---

## 🖥️ System Requirements

### **Minimum Requirements**
- **OS**: Windows 10/11 (64-bit)
- **Python**: 3.10 or higher
- **RAM**: 4GB (8GB recommended)
- **Internet**: Stable broadband connection (minimum 2 Mbps)
- **Screen Resolution**: 1366x768 or higher

### **Required Accounts**
- Active Kotak Securities trading account
- Kotak Neo API credentials (Token)
- Valid TOTP authenticator setup

