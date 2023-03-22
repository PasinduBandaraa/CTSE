# CTSE

1. Install the react-native-datetimepicker library using npm or yarn.

```bash
npm install @react-native-community/datetimepicker
```

2. Import the DateTimePicker component in your React Native file.

```javascript
import DateTimePicker from '@react-native-community/datetimepicker';
```

3. Create a state to store the selected date and time.

```javascript
const [date, setDate] = useState(new Date());
```

4. Create a function that will handle the date and time change.

```javascript
const handleDateChange = (event, selectedDate) => {
  const currentDate = selectedDate || date;
  setDate(currentDate);
};
```

5. Render the DateTimePicker component.

```javascript
<DateTimePicker
  testID="dateTimePicker"
  value={date}
  mode={'datetime'}
  is24Hour={true}
  display="default"
  onChange={handleDateChange}
/>
```

Customize the DateTimePicker component according to your requirements.

You can customize the mode prop to display only date or time, or both. You can also customize the display prop to show a calendar or a spinner.

Once you have the selected date and time, you can use it to update your laboratory report in your CRUD operation.
