'use client'

import { useState } from 'react'
import { Select } from '@/components/ui/select'
import { Button } from '@/components/ui/button'

const productionLines = Array.from({ length: 150 }, (_, i) => ({
  value: `line-${i + 1}`,
  label: `Production Line ${i + 1}`
}))

export default function TrainingCenter() {
  const [selectedLine, setSelectedLine] = useState('')

  return (
    <div className="container mx-auto px-4 py-8">
      <h1 className="text-3xl font-bold mb-4">Training Center</h1>
      <div className="max-w-md">
        <Select
          options={productionLines}
          value={selectedLine}
          onChange={(value) => setSelectedLine(value)}
          placeholder="Select a production line"
          className="mb-4"
        />
        <Button disabled={!selectedLine}>Start Training</Button>
      </div>
    </div>
  )
}

