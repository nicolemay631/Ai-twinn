import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";
import { Input } from "@/components/ui/input";

export default function CBTCoachLanding() {
  return (
    <div className="min-h-screen bg-gradient-to-b from-blue-50 to-white p-6 flex flex-col items-center text-center">
      <h1 className="text-4xl font-bold text-blue-800 mt-10">Your Personal AI CBT Coach</h1>
      <p className="text-lg text-gray-600 mt-4 max-w-xl">
        Feel better, one daily chat at a time. Built for those navigating depression or anxiety,
        this AI-powered companion offers daily support, reflection, and science-backed wellness guidance.
      </p>

      <div className="mt-10 grid grid-cols-1 md:grid-cols-3 gap-6 max-w-5xl w-full">
        <Card className="rounded-2xl shadow-md">
          <CardContent className="p-6">
            <h2 className="text-xl font-semibold text-blue-700">Starter</h2>
            <p className="text-gray-600 mt-2">Free daily prompts and journaling</p>
            <p className="text-2xl font-bold mt-4">$0/mo</p>
            <Button className="mt-4 w-full">Get Started</Button>
          </CardContent>
        </Card>

        <Card className="rounded-2xl shadow-md border-blue-400 border-2">
          <CardContent className="p-6">
            <h2 className="text-xl font-semibold text-blue-700">Growth</h2>
            <p className="text-gray-600 mt-2">Unlimited AI support + product discounts</p>
            <p className="text-2xl font-bold mt-4">$9/mo</p>
            <Button className="mt-4 w-full">Subscribe</Button>
          </CardContent>
        </Card>

        <Card className="rounded-2xl shadow-md">
          <CardContent className="p-6">
            <h2 className="text-xl font-semibold text-blue-700">Full Support</h2>
            <p className="text-gray-600 mt-2">AI + group check-ins and coaching sessions</p>
            <p className="text-2xl font-bold mt-4">$29/mo</p>
            <Button className="mt-4 w-full">Join Now</Button>
          </CardContent>
        </Card>
      </div>

      <div className="mt-16 bg-white shadow-lg rounded-xl p-8 max-w-2xl w-full">
        <h3 className="text-2xl font-bold text-blue-800 mb-4">Try a 7-Day Mental Reset for Free</h3>
        <p className="text-gray-600 mb-4">Enter your email to get started with your AI twin today.</p>
        <div className="flex gap-2 justify-center">
          <Input placeholder="you@example.com" className="w-full max-w-md" />
          <Button>Start Now</Button>
        </div>
      </div>
    </div>
  );
}
