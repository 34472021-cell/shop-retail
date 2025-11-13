import React, { useState } from 'react';
import { ShoppingCart, Plus, Minus, Trash2, Store } from 'lucide-react';

export default function ShopOrderSystem() {
  const [items] = useState([
    { id: 1, name: 'Coconut Cakes', price: 10, available: 50 },
    { id: 2, name: 'Mandazi', price: 5, available: 100 },
    { id: 3, name: 'KDF Bread', price: 15, available: 30 },
    { id: 4, name: 'Normal Bread', price: 12, available: 40 },
    { id: 5, name: 'Chapati', price: 10, available: 60 },
    { id: 6, name: 'Samosa', price: 20, available: 45 },
    { id: 7, name: 'Milk (Small)', price: 30, available: 35 },
    { id: 8, name: 'Milk (Large)', price: 60, available: 25 }
  ]);

  const [cart, setCart] = useState([]);
  const [customerName, setCustomerName] = useState('');
  const [phoneNumber, setPhoneNumber] = useState('');
  const [destination, setDestination] = useState('');
  const [orderPlaced, setOrderPlaced] = useState(false);

  const addToCart = (item) => {
    const existingItem = cart.find(cartItem => cartItem.id === item.id);
    
    if (existingItem) {
      if (existingItem.quantity < item.available) {
        setCart(cart.map(cartItem =>
          cartItem.id === item.id
            ? { ...cartItem, quantity: cartItem.quantity + 1 }
            : cartItem
        ));
      } else {
        alert(`Only ${item.available} ${item.name} available!`);
      }
    } else {
      setCart([...cart, { ...item, quantity: 1 }]);
    }
  };

  const updateQuantity = (id, change) => {
    const item = items.find(i => i.id === id);
    setCart(cart.map(cartItem => {
      if (cartItem.id === id) {
        const newQuantity = cartItem.quantity + change;
        if (newQuantity > item.available) {
          alert(`Only ${item.available} ${item.name} available!`);
          return cartItem;
        }
        return { ...cartItem, quantity: Math.max(0, newQuantity) };
      }
      return cartItem;
    }).filter(cartItem => cartItem.quantity > 0));
  };

  const removeFromCart = (id) => {
    setCart(cart.filter(item => item.id !== id));
  };

  const getTotalPrice = () => {
    return cart.reduce((total, item) => total + (item.price * item.quantity), 0);
  };

  const placeOrder = () => {
    if (!customerName || !phoneNumber || !destination) {
      alert('Please fill in all delivery details!');
      return;
    }
    if (cart.length === 0) {
      alert('Please add items to your cart!');
      return;
    }
    setOrderPlaced(true);
  };

  const resetOrder = () => {
    setCart([]);
    setCustomerName('');
    setPhoneNumber('');
    setDestination('');
    setOrderPlaced(false);
  };

  if (orderPlaced) {
    return (
      <div className="min-h-screen bg-black p-4">
        <div className="max-w-2xl mx-auto bg-gradient-to-br from-gray-900 to-black rounded-lg shadow-2xl p-8 text-center border-2 border-green-500" style={{boxShadow: '0 0 30px rgba(34, 197, 94, 0.5)'}}>
          <div className="text-6xl mb-4">✅</div>
          <h2 className="text-3xl font-bold text-green-400 mb-4" style={{textShadow: '0 0 20px rgba(34, 197, 94, 0.8)'}}>Order Placed Successfully!</h2>
          
          <div className="bg-gray-900 p-6 rounded-lg mb-6 text-left border border-green-500" style={{boxShadow: '0 0 15px rgba(34, 197, 94, 0.3)'}}>
            <h3 className="font-bold text-xl mb-4 text-green-400">Order Summary</h3>
            <p className="mb-2 text-gray-300"><strong className="text-green-400">Customer:</strong> {customerName}</p>
            <p className="mb-2 text-gray-300"><strong className="text-green-400">Phone:</strong> {phoneNumber}</p>
            <p className="mb-2 text-gray-300"><strong className="text-green-400">Delivery To:</strong> {destination}</p>
            <p className="mb-4 text-green-400 font-semibold">💰 Payment: Cash on Delivery</p>
            
            <div className="border-t border-green-500 pt-4">
              <h4 className="font-semibold mb-2 text-green-400">Items:</h4>
              {cart.map(item => (
                <div key={item.id} className="flex justify-between mb-2 text-gray-300">
                  <span>{item.name} x{item.quantity}</span>
                  <span className="text-green-400">KSh {item.price * item.quantity}</span>
                </div>
              ))}
              <div className="border-t border-green-500 pt-2 mt-2 font-bold flex justify-between">
                <span className="text-green-400">Total:</span>
                <span className="text-green-400 text-xl">KSh {getTotalPrice()}</span>
              </div>
            </div>
          </div>
          
          <button
            onClick={resetOrder}
            className="bg-green-500 text-black px-8 py-3 rounded-lg hover:bg-green-400 transition font-bold"
            style={{boxShadow: '0 0 20px rgba(34, 197, 94, 0.6)'}}
          >
            Place New Order
          </button>
        </div>
      </div>
    );
  }

  return (
    <div className="min-h-screen bg-black p-4">
      <div className="max-w-6xl mx-auto">
        <div className="bg-gradient-to-r from-gray-900 to-black rounded-lg shadow-2xl p-6 mb-6 border-2 border-green-500" style={{boxShadow: '0 0 30px rgba(34, 197, 94, 0.5)'}}>
          <h1 className="text-4xl font-bold text-green-400 mb-2 flex items-center gap-3" style={{textShadow: '0 0 20px rgba(34, 197, 94, 0.8)'}}>
            <Store className="text-green-400" size={40} />
            MamaJohn's Shop
          </h1>
          <p className="text-gray-300 text-lg">Fresh baked goods delivered to your door</p>
        </div>

        <div className="grid md:grid-cols-2 gap-6">
          {/* Available Items */}
          <div className="bg-gradient-to-br from-gray-900 to-black rounded-lg shadow-2xl p-6 border-2 border-green-500" style={{boxShadow: '0 0 25px rgba(34, 197, 94, 0.4)'}}>
            <h2 className="text-2xl font-bold text-green-400 mb-4" style={{textShadow: '0 0 15px rgba(34, 197, 94, 0.6)'}}>Available Items</h2>
            <div className="space-y-3">
              {items.map(item => (
                <div key={item.id} className="border-2 border-gray-700 rounded-lg p-4 hover:border-green-500 transition bg-gray-900" style={{boxShadow: '0 0 10px rgba(0, 0, 0, 0.5)'}}>
                  <div className="flex justify-between items-center mb-2">
                    <h3 className="font-semibold text-lg text-gray-200">{item.name}</h3>
                    <span className="text-green-400 font-bold text-lg" style={{textShadow: '0 0 10px rgba(34, 197, 94, 0.6)'}}>KSh {item.price}</span>
                  </div>
                  <div className="flex justify-between items-center">
                    <span className="text-sm text-gray-400">Available: {item.available}</span>
                    <button
                      onClick={() => addToCart(item)}
                      className="bg-green-500 text-black px-4 py-2 rounded hover:bg-green-400 transition flex items-center gap-1 font-bold"
                      style={{boxShadow: '0 0 15px rgba(34, 197, 94, 0.5)'}}
                    >
                      <Plus size={16} /> Add
                    </button>
                  </div>
                </div>
              ))}
            </div>
          </div>

          {/* Cart and Order Details */}
          <div className="space-y-6">
            {/* Cart */}
            <div className="bg-gradient-to-br from-gray-900 to-black rounded-lg shadow-2xl p-6 border-2 border-green-500" style={{boxShadow: '0 0 25px rgba(34, 197, 94, 0.4)'}}>
              <h2 className="text-2xl font-bold text-green-400 mb-4 flex items-center gap-2" style={{textShadow: '0 0 15px rgba(34, 197, 94, 0.6)'}}>
                <ShoppingCart size={28} />
                Your Cart
              </h2>
              {cart.length === 0 ? (
                <p className="text-gray-500 text-center py-8">Your cart is empty</p>
              ) : (
                <div className="space-y-3">
                  {cart.map(item => (
                    <div key={item.id} className="border border-gray-700 rounded-lg p-3 bg-gray-900">
                      <div className="flex justify-between items-center mb-2">
                        <h3 className="font-semibold text-gray-200">{item.name}</h3>
                        <button
                          onClick={() => removeFromCart(item.id)}
                          className="text-red-500 hover:text-red-400"
                        >
                          <Trash2 size={18} />
                        </button>
                      </div>
                      <div className="flex justify-between items-center">
                        <div className="flex items-center gap-2">
                          <button
                            onClick={() => updateQuantity(item.id, -1)}
                            className="bg-gray-700 p-1 rounded hover:bg-gray-600 text-green-400"
                          >
                            <Minus size={16} />
                          </button>
                          <span className="font-semibold text-green-400">{item.quantity}</span>
                          <button
                            onClick={() => updateQuantity(item.id, 1)}
                            className="bg-gray-700 p-1 rounded hover:bg-gray-600 text-green-400"
                          >
                            <Plus size={16} />
                          </button>
                        </div>
                        <span className="font-bold text-green-400">KSh {item.price * item.quantity}</span>
                      </div>
                    </div>
                  ))}
                  <div className="border-t border-green-500 pt-3 mt-3">
                    <div className="flex justify-between items-center text-xl font-bold">
                      <span className="text-green-400">Total:</span>
                      <span className="text-green-400 text-2xl" style={{textShadow: '0 0 15px rgba(34, 197, 94, 0.8)'}}>KSh {getTotalPrice()}</span>
                    </div>
                  </div>
                </div>
              )}
            </div>

            {/* Delivery Details */}
            <div className="bg-gradient-to-br from-gray-900 to-black rounded-lg shadow-2xl p-6 border-2 border-green-500" style={{boxShadow: '0 0 25px rgba(34, 197, 94, 0.4)'}}>
              <h2 className="text-2xl font-bold text-green-400 mb-4" style={{textShadow: '0 0 15px rgba(34, 197, 94, 0.6)'}}>Delivery Details</h2>
              
              <div className="bg-green-900 border border-green-500 rounded-lg p-3 mb-4" style={{boxShadow: '0 0 10px rgba(34, 197, 94, 0.3)'}}>
                <p className="text-green-300 text-center font-semibold">💰 Payment on Delivery</p>
                <p className="text-green-400 text-sm text-center">Pay cash when you receive your order</p>
              </div>
              <div className="space-y-4">
                <div>
                  <label className="block text-sm font-semibold mb-2 text-green-400">Customer Name</label>
                  <input
                    type="text"
                    value={customerName}
                    onChange={(e) => setCustomerName(e.target.value)}
                    className="w-full border-2 border-gray-700 rounded-lg px-4 py-2 focus:outline-none focus:ring-2 focus:ring-green-500 bg-gray-900 text-gray-200"
                    placeholder="Enter your name"
                  />
                </div>
                <div>
                  <label className="block text-sm font-semibold mb-2 text-green-400">Phone Number</label>
                  <input
                    type="tel"
                    value={phoneNumber}
                    onChange={(e) => setPhoneNumber(e.target.value)}
                    className="w-full border-2 border-gray-700 rounded-lg px-4 py-2 focus:outline-none focus:ring-2 focus:ring-green-500 bg-gray-900 text-gray-200"
                    placeholder="07XX XXX XXX"
                  />
                </div>
                <div>
                  <label className="block text-sm font-semibold mb-2 text-green-400">Delivery Destination</label>
                  <input
                    type="text"
                    value={destination}
                    onChange={(e) => setDestination(e.target.value)}
                    className="w-full border-2 border-gray-700 rounded-lg px-4 py-2 focus:outline-none focus:ring-2 focus:ring-green-500 bg-gray-900 text-gray-200"
                    placeholder="Enter delivery address"
                  />
                </div>
                <button
                  onClick={placeOrder}
                  className="w-full bg-green-500 text-black py-3 rounded-lg hover:bg-green-400 transition font-bold text-lg"
                  style={{boxShadow: '0 0 25px rgba(34, 197, 94, 0.6)'}}
                >
                  Place Order
                </button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  );
}
